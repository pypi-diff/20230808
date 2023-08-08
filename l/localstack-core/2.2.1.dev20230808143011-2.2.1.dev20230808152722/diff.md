# Comparing `tmp/localstack-core-2.2.1.dev20230808143011.tar.gz` & `tmp/localstack-core-2.2.1.dev20230808152722.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.2.1.dev20230808143011.tar", last modified: Tue Aug  8 14:30:30 2023, max compression
+gzip compressed data, was "localstack-core-2.2.1.dev20230808152722.tar", last modified: Tue Aug  8 15:27:38 2023, max compression
```

## Comparing `localstack-core-2.2.1.dev20230808143011.tar` & `localstack-core-2.2.1.dev20230808152722.tar`

### file list

```diff
@@ -1,906 +1,906 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.772967 localstack-core-2.2.1.dev20230808143011/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15463 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-08 14:30:30.772967 localstack-core-2.2.1.dev20230808143011/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11767 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.636969 localstack-core-2.2.1.dev20230808143011/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.640969 localstack-core-2.2.1.dev20230808143011/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-08-08 14:30:11.000000 localstack-core-2.2.1.dev20230808143011/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.640969 localstack-core-2.2.1.dev20230808143011/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    89045 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   761978 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.656969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72158 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68029 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   135061 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15408 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/scheduler/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10043 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.660969 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22962 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.664969 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10618 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.664969 localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49981 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14655 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.664969 localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31104 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.664969 localstack-core-2.2.1.dev20230808143011/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28990 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51644 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.668969 localstack-core-2.2.1.dev20230808143011/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.668969 localstack-core-2.2.1.dev20230808143011/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.668969 localstack-core-2.2.1.dev20230808143011/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.668969 localstack-core-2.2.1.dev20230808143011/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6236 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.668969 localstack-core-2.2.1.dev20230808143011/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.668969 localstack-core-2.2.1.dev20230808143011/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8744 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.668969 localstack-core-2.2.1.dev20230808143011/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.672969 localstack-core-2.2.1.dev20230808143011/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.672969 localstack-core-2.2.1.dev20230808143011/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.672969 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    66867 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14958 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3035 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12244 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91066 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.676969 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24649 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.676969 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.676969 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20045 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.676969 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   156015 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.676969 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3587 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9266 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.680969 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12539 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50605 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.680969 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33125 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20288 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      943 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2522 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6543 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2251 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5628 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21069 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2570 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3350 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8604 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27126 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3201 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2876 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3337 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4863 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1437 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3655 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13424 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6535 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4826 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10793 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5626 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41357 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26078 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.680969 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15528 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.680969 localstack-core-2.2.1.dev20230808143011/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.684969 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.684969 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4547 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6060 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.684969 localstack-core-2.2.1.dev20230808143011/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.684969 localstack-core-2.2.1.dev20230808143011/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.684969 localstack-core-2.2.1.dev20230808143011/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.684969 localstack-core-2.2.1.dev20230808143011/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24704 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.684969 localstack-core-2.2.1.dev20230808143011/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.684969 localstack-core-2.2.1.dev20230808143011/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.684969 localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6650 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.688969 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.688969 localstack-core-2.2.1.dev20230808143011/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.688969 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.688969 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12249 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.688969 localstack-core-2.2.1.dev20230808143011/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.688969 localstack-core-2.2.1.dev20230808143011/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.688969 localstack-core-2.2.1.dev20230808143011/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.688969 localstack-core-2.2.1.dev20230808143011/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.688969 localstack-core-2.2.1.dev20230808143011/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.692969 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3028 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/exceptions.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.692969 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68165 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15016 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17710 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    95039 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34001 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/provider_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23872 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.692969 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22373 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49285 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.692969 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/storage/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/storage/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4979 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/storage/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/storage/ephemeral.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.692969 localstack-core-2.2.1.dev20230808143011/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.692969 localstack-core-2.2.1.dev20230808143011/localstack/services/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/scheduler/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/scheduler/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/scheduler/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.692969 localstack-core-2.2.1.dev20230808143011/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.692969 localstack-core-2.2.1.dev20230808143011/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.692969 localstack-core-2.2.1.dev20230808143011/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54706 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.696969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1531 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.700969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.700969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      744 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.700969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.700969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.700969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.700969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.700969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.700969 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.728968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.728968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.728968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.728968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.728968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.728968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.736968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4331 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.740968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6029 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.744968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.744968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.744968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10660 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2954 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1250 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1359 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3273 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6915 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1602 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1184 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7164 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1639 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6068 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5345 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5863 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5049 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9094 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5199 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.752968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.756968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3387 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1614 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.756968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.756968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.756968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1682 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.756968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.756968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5069 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.756968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4937 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1539 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1711 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      860 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32935 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8885 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2611 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14214 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.760968 localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7949 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.764968 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68881 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1827 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/marking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.764968 localstack-core-2.2.1.dev20230808143011/localstack/testing/scenario/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/scenario/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6860 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/scenario/provisioning.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.764968 localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28239 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.768967 localstack-core-2.2.1.dev20230808143011/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.768967 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.768967 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17941 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11940 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7674 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26833 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.768967 localstack-core-2.2.1.dev20230808143011/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.772967 localstack-core-2.2.1.dev20230808143011/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48572 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33233 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4113 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.772967 localstack-core-2.2.1.dev20230808143011/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.772967 localstack-core-2.2.1.dev20230808143011/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:30:30.772967 localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-08 14:30:30.000000 localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40753 2023-08-08 14:30:30.000000 localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 14:30:30.000000 localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5444 2023-08-08 14:30:30.000000 localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 14:30:24.000000 localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5539 2023-08-08 14:30:24.000000 localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2894 2023-08-08 14:30:30.000000 localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-08-08 14:30:30.000000 localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3275 2023-08-08 14:30:30.772967 localstack-core-2.2.1.dev20230808143011/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-08-08 13:53:40.000000 localstack-core-2.2.1.dev20230808143011/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.631577 localstack-core-2.2.1.dev20230808152722/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15463 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-08 15:27:38.631577 localstack-core-2.2.1.dev20230808152722/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11767 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.179586 localstack-core-2.2.1.dev20230808152722/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.183586 localstack-core-2.2.1.dev20230808152722/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-08-08 15:27:22.000000 localstack-core-2.2.1.dev20230808152722/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.195585 localstack-core-2.2.1.dev20230808152722/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4215 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.195585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.195585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.195585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.199585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.199585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    89045 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.199585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.203585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.203585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.207585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.207585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   761978 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.211585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.211585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.211585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.215585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.215585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.215585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.219585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72158 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.219585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.219585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.223585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.223585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.223585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.223585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68029 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.227585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    56394 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.227585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   135615 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.227585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.231585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15408 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/scheduler/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.231585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.231585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.231585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.235585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.235585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.235585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.235585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10043 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.239585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.239585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.239585 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40756 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22962 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9179 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.251584 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10618 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.255584 localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49981 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14655 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.259584 localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32580 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.263584 localstack-core-2.2.1.dev20230808152722/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28990 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51644 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8101 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.263584 localstack-core-2.2.1.dev20230808152722/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.263584 localstack-core-2.2.1.dev20230808152722/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.267584 localstack-core-2.2.1.dev20230808152722/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.275584 localstack-core-2.2.1.dev20230808152722/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6236 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.275584 localstack-core-2.2.1.dev20230808152722/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.279584 localstack-core-2.2.1.dev20230808152722/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8744 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.287584 localstack-core-2.2.1.dev20230808152722/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.291584 localstack-core-2.2.1.dev20230808152722/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.295583 localstack-core-2.2.1.dev20230808152722/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.303583 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    66867 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40175 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14958 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3035 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12244 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91066 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.315583 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24649 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.319583 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.323583 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20045 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91622 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72372 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4172 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.327583 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   156015 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.335583 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3587 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9266 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.343582 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12539 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50605 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7987 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14107 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.363582 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33125 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20288 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      943 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2522 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6543 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2251 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5628 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21069 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2570 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3350 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8604 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27126 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3201 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2876 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3337 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4863 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2751 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1437 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3655 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13424 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6535 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8787 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4826 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10793 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5626 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41357 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26078 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.363582 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15528 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16227 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.367582 localstack-core-2.2.1.dev20230808152722/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.371582 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73160 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6110 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10655 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.375582 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4547 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6060 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.375582 localstack-core-2.2.1.dev20230808152722/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20637 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.379582 localstack-core-2.2.1.dev20230808152722/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.379582 localstack-core-2.2.1.dev20230808152722/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24701 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.383582 localstack-core-2.2.1.dev20230808152722/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31768 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24704 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.383582 localstack-core-2.2.1.dev20230808152722/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20341 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.383582 localstack-core-2.2.1.dev20230808152722/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.387582 localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6650 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7002 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.391582 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.395582 localstack-core-2.2.1.dev20230808152722/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16343 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.399582 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.399582 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12249 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.399582 localstack-core-2.2.1.dev20230808152722/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.403581 localstack-core-2.2.1.dev20230808152722/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.403581 localstack-core-2.2.1.dev20230808152722/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.403581 localstack-core-2.2.1.dev20230808152722/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.407581 localstack-core-2.2.1.dev20230808152722/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33621 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.415581 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3028 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/exceptions.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.419581 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68165 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15016 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17710 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30110 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    95039 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34001 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/provider_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23872 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.423581 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22307 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68712 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.423581 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/storage/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/storage/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4979 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/storage/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/storage/ephemeral.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.423581 localstack-core-2.2.1.dev20230808152722/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.427581 localstack-core-2.2.1.dev20230808152722/localstack/services/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/scheduler/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/scheduler/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/scheduler/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.427581 localstack-core-2.2.1.dev20230808152722/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27787 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.427581 localstack-core-2.2.1.dev20230808152722/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22744 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.431581 localstack-core-2.2.1.dev20230808152722/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      823 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5617 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45605 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55136 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.439581 localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54706 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.439581 localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16588 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.439581 localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.443580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.443580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.443580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.447580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.451580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.451580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.455580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1531 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.459580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.463580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      744 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.463580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.463580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.463580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.467580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.467580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.471580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.475580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.479580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.479580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.487580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.487580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.491580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.495580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.499580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.499580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.499580 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.503579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.503579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.503579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.503579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.507579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.507579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4331 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.511579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6029 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.515579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.519579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.519579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.523579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.523579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10660 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.527579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.527579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.531579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2954 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1250 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1359 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3273 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6915 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.531579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1602 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1184 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7164 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.531579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1639 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.535579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.539579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6068 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5345 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5863 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5049 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3342 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9094 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3158 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5199 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.539579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1905 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.543579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3387 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1614 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.543579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.543579 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.547578 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1682 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.551578 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.551578 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5069 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.551578 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4937 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.551578 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1539 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1711 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.555578 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      860 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.555578 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32935 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.559578 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.563578 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8885 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2611 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14214 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4332 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.563578 localstack-core-2.2.1.dev20230808152722/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.563578 localstack-core-2.2.1.dev20230808152722/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.563578 localstack-core-2.2.1.dev20230808152722/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.563578 localstack-core-2.2.1.dev20230808152722/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13543 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.567578 localstack-core-2.2.1.dev20230808152722/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.567578 localstack-core-2.2.1.dev20230808152722/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.571578 localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7949 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.579578 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68881 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1827 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/marking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.579578 localstack-core-2.2.1.dev20230808152722/localstack/testing/scenario/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/scenario/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6860 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/scenario/provisioning.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.583578 localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28239 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.607577 localstack-core-2.2.1.dev20230808152722/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.615577 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.619577 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13553 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17941 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11940 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2740 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7674 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26833 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.623577 localstack-core-2.2.1.dev20230808152722/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6170 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.623577 localstack-core-2.2.1.dev20230808152722/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48572 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33233 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33378 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4113 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.627577 localstack-core-2.2.1.dev20230808152722/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.631577 localstack-core-2.2.1.dev20230808152722/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23609 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:27:38.631577 localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-08-08 15:27:38.000000 localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40753 2023-08-08 15:27:38.000000 localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 15:27:38.000000 localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5444 2023-08-08 15:27:38.000000 localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 15:27:32.000000 localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5539 2023-08-08 15:27:32.000000 localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2894 2023-08-08 15:27:38.000000 localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-08-08 15:27:38.000000 localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3275 2023-08-08 15:27:38.631577 localstack-core-2.2.1.dev20230808152722/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-08-08 14:50:47.000000 localstack-core-2.2.1.dev20230808152722/setup.py
```

### Comparing `localstack-core-2.2.1.dev20230808143011/LICENSE.txt` & `localstack-core-2.2.1.dev20230808152722/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/Makefile` & `localstack-core-2.2.1.dev20230808152722/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/PKG-INFO` & `localstack-core-2.2.1.dev20230808152722/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230808143011
+Version: 2.2.1.dev20230808152722
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230808143011/README.md` & `localstack-core-2.2.1.dev20230808152722/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/bin/localstack` & `localstack-core-2.2.1.dev20230808152722/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/bin/localstack-supervisor` & `localstack-core-2.2.1.dev20230808152722/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/accounts.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/acm/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/config/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/core.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/es/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/events/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/iam/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/kms/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/logs/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/route53/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/s3/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/s3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -804,14 +804,37 @@
 class BucketNotEmpty(ServiceException):
     code: str = "BucketNotEmpty"
     sender_fault: bool = False
     status_code: int = 409
     BucketName: Optional[BucketName]
 
 
+ProposedSize = int
+MinSizeAllowed = int
+
+
+class EntityTooSmall(ServiceException):
+    code: str = "EntityTooSmall"
+    sender_fault: bool = False
+    status_code: int = 400
+    ETag: Optional[ETag]
+    MinSizeAllowed: Optional[MinSizeAllowed]
+    PartNumber: Optional[PartNumber]
+    ProposedSize: Optional[ProposedSize]
+
+
+class InvalidPart(ServiceException):
+    code: str = "InvalidPart"
+    sender_fault: bool = False
+    status_code: int = 400
+    ETag: Optional[ETag]
+    UploadId: Optional[MultipartUploadId]
+    PartNumber: Optional[PartNumber]
+
+
 AbortDate = datetime
 
 
 class AbortIncompleteMultipartUpload(TypedDict, total=False):
     DaysAfterInitiation: Optional[DaysAfterInitiation]
```

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/scheduler/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/ses/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/sns/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/sts/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/support/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/swf/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/app.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/chain.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/client.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/connect.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/forwarder.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/gateway.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/analytics.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/auth.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/codec.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/cors.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/fallback.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/internal.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/legacy.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/logging.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/proxy.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/region.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/routes.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/service.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/mocking.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/op_router.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/parser.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/serializer.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/service_router.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/protocol/validate.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/proxy.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/scaffold.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/asgi.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/edge.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/hypercorn.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/werkzeug.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/serving/wsgi.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/skeleton.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/spec-patches.json` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/spec-patches.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.974025974025974%*

 * *Differences: {"'s3/2006-03-01/service-2'": "{insert: [(73, OrderedDict([('op', 'add'), ('path', "*

 * *                              "'/shapes/MinSizeAllowed'), ('value', OrderedDict([('type', "*

 * *                              "'long')]))])), (74, OrderedDict([('op', 'add'), ('path', "*

 * *                              "'/shapes/ProposedSize'), ('value', OrderedDict([('type', "*

 * *                              "'long')]))])), (75, OrderedDict([('op', 'add'), ('path', "*

 * *                              "'/shapes/EntityTooSmall'), ('value […]*

```diff
@@ -928,10 +928,67 @@
                 "members": {
                     "BucketName": {
                         "shape": "BucketName"
                     }
                 },
                 "type": "structure"
             }
+        },
+        {
+            "op": "add",
+            "path": "/shapes/MinSizeAllowed",
+            "value": {
+                "type": "long"
+            }
+        },
+        {
+            "op": "add",
+            "path": "/shapes/ProposedSize",
+            "value": {
+                "type": "long"
+            }
+        },
+        {
+            "op": "add",
+            "path": "/shapes/EntityTooSmall",
+            "value": {
+                "documentation": "<p>Your proposed upload is smaller than the minimum allowed object size. Each part must be at least 5 MB in size, except the last part.</p>",
+                "exception": true,
+                "members": {
+                    "ETag": {
+                        "shape": "ETag"
+                    },
+                    "MinSizeAllowed": {
+                        "shape": "MinSizeAllowed"
+                    },
+                    "PartNumber": {
+                        "shape": "PartNumber"
+                    },
+                    "ProposedSize": {
+                        "shape": "ProposedSize"
+                    }
+                },
+                "type": "structure"
+            }
+        },
+        {
+            "op": "add",
+            "path": "/shapes/InvalidPart",
+            "value": {
+                "documentation": "<p>One or more of the specified parts could not be found. The part might not have been uploaded, or the specified entity tag might not have matched the part's entity tag.</p>",
+                "exception": true,
+                "members": {
+                    "ETag": {
+                        "shape": "ETag"
+                    },
+                    "PartNumber": {
+                        "shape": "PartNumber"
+                    },
+                    "UploadId": {
+                        "shape": "MultipartUploadId"
+                    }
+                },
+                "type": "structure"
+            }
         }
     ]
 }
```

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/spec.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/aws/trace.py` & `localstack-core-2.2.1.dev20230808152722/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/cli/localstack.py` & `localstack-core-2.2.1.dev20230808152722/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/cli/lpm.py` & `localstack-core-2.2.1.dev20230808152722/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/cli/plugin.py` & `localstack-core-2.2.1.dev20230808152722/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/cli/plugins.py` & `localstack-core-2.2.1.dev20230808152722/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/cli/profiles.py` & `localstack-core-2.2.1.dev20230808152722/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/config.py` & `localstack-core-2.2.1.dev20230808152722/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/constants.py` & `localstack-core-2.2.1.dev20230808152722/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/deprecations.py` & `localstack-core-2.2.1.dev20230808152722/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/extensions/api/aws.py` & `localstack-core-2.2.1.dev20230808152722/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/extensions/api/extension.py` & `localstack-core-2.2.1.dev20230808152722/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/adapters.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/asgi.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/client.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/dispatcher.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/hypercorn.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/proxy.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/request.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/resource.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/response.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/http/router.py` & `localstack-core-2.2.1.dev20230808152722/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/logging/format.py` & `localstack-core-2.2.1.dev20230808152722/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/logging/setup.py` & `localstack-core-2.2.1.dev20230808152722/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/packages/__init__.py` & `localstack-core-2.2.1.dev20230808152722/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/packages/api.py` & `localstack-core-2.2.1.dev20230808152722/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/packages/core.py` & `localstack-core-2.2.1.dev20230808152722/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/packages/debugpy.py` & `localstack-core-2.2.1.dev20230808152722/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/packages/ffmpeg.py` & `localstack-core-2.2.1.dev20230808152722/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/packages/terraform.py` & `localstack-core-2.2.1.dev20230808152722/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/plugins.py` & `localstack-core-2.2.1.dev20230808152722/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/runtime/analytics.py` & `localstack-core-2.2.1.dev20230808152722/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/runtime/hooks.py` & `localstack-core-2.2.1.dev20230808152722/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/runtime/init.py` & `localstack-core-2.2.1.dev20230808152722/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/runtime/main.py` & `localstack-core-2.2.1.dev20230808152722/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/runtime/shutdown.py` & `localstack-core-2.2.1.dev20230808152722/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/acm/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/context.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/helpers.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/integration.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/invocations.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/patches.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/router_asf.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/apigateway/templates.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/api_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/hooks.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/packages.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/plugins.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/deploy.html` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/quirks.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/template_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/template_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/types.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/events.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/packages.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/provider_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/service_models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudformation/stores.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/cloudwatch/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/packages.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/server.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodb/utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/ec2/exceptions.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/ec2/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/ec2/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/edge.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/es/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/events/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/events/scheduler.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/firehose/mappers.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/firehose/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/firehose/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/generic_proxy.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/iam/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack-core-2.2.1.dev20230808152722/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/infra.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/internal.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/packages.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kinesis/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kms/local_kms_server.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kms/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kms/packages.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kms/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/kms/utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/logs/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/logs/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/messages.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/moto.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/motoserver.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/cluster.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/packages.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/opensearch/versions.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/plugins.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/providers.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/redshift/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/route53/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/route53resolver/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/route53resolver/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/route53resolver/utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/codec.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/constants.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/cors.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/exceptions.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/multipart_content.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/s3_listener.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/s3_starter.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/legacy/s3_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/legacy/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/notifications.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/presigned_url.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/provider_stream.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/provider_stream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 import logging
 from collections import defaultdict
 from datetime import datetime
 from secrets import token_urlsafe
 from typing import Literal, Optional, Union
 
 from localstack import config
-from localstack.aws.api.s3 import (  # EntityTooSmall,; InvalidPart,
+from localstack.aws.api.s3 import (
     AccountId,
     AnalyticsConfiguration,
     AnalyticsId,
     BucketAccelerateStatus,
     BucketName,
     BucketRegion,
     BucketVersioningStatus,
     ChecksumAlgorithm,
     CompletedPartList,
     CORSConfiguration,
+    EntityTooSmall,
     ETag,
     Expiration,
     IntelligentTieringConfiguration,
     IntelligentTieringId,
     InvalidArgument,
+    InvalidPart,
     LifecycleRules,
     LoggingEnabled,
     Metadata,
     MethodNotAllowed,
     MultipartUploadId,
     NoSuchKey,
     NoSuchVersion,
@@ -401,36 +403,34 @@
         pos = 0
         for index, part in enumerate(parts):
             part_number = part["PartNumber"]
             part_etag = part["ETag"].strip('"')
 
             s3_part = self.parts.get(part_number)
             if not s3_part or s3_part.etag != part_etag:
-                raise
-                # raise InvalidPart(
-                #     "One or more of the specified parts could not be found.  The part may not have been uploaded, or the specified entity tag may not match the part's entity tag.",
-                #     ETag=part_etag,
-                #     PartNumber=part_number,
-                #     UploadId=self.id,
-                # )
+                raise InvalidPart(
+                    "One or more of the specified parts could not be found.  The part may not have been uploaded, or the specified entity tag may not match the part's entity tag.",
+                    ETag=part_etag,
+                    PartNumber=part_number,
+                    UploadId=self.id,
+                )
 
             # TODO: this part is currently not implemented, time permitting
             # part_checksum = part.get(checksum_key) if self.object.checksum_algorithm else None
             # if part_checksum and part_checksum != s3_part.checksum_value:
             #     raise Exception()
 
             if index != last_part_index and s3_part.size < S3_UPLOAD_PART_MIN_SIZE:
-                raise
-                # raise EntityTooSmall(
-                #     "Your proposed upload is smaller than the minimum allowed size",
-                #     ETag=part_etag,
-                #     PartNumber=part_number,
-                #     MinSizeAllowed=S3_UPLOAD_PART_MIN_SIZE,
-                #     ProposedSize=s3_part.size,
-                # )
+                raise EntityTooSmall(
+                    "Your proposed upload is smaller than the minimum allowed size",
+                    ETag=part_etag,
+                    PartNumber=part_number,
+                    MinSizeAllowed=S3_UPLOAD_PART_MIN_SIZE,
+                    ProposedSize=s3_part.size,
+                )
 
             object_etag.update(bytes.fromhex(s3_part.etag))
             # TODO verify this, it seems wrong
             self.object.parts.append((pos, s3_part.size))
 
             multipart_etag = f"{object_etag.hexdigest()}-{len(parts)}"
             self.object.etag = multipart_etag
```

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sns/provider.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1232 +1,1018 @@
-import base64
-import datetime
+import json
 import logging
-from secrets import token_urlsafe
+from typing import Dict, List
 
-from localstack import config
-from localstack.aws.api import CommonServiceException, RequestContext, handler
-from localstack.aws.api.s3 import (
-    MFA,
-    AccountId,
-    Bucket,
-    BucketAlreadyExists,
-    BucketAlreadyOwnedByYou,
-    BucketName,
-    BucketNotEmpty,
-    BypassGovernanceRetention,
-    ChecksumAlgorithm,
-    CommonPrefix,
-    CopyObjectOutput,
-    CopyObjectRequest,
-    CopyObjectResult,
-    CreateBucketOutput,
-    CreateBucketRequest,
-    Delete,
-    DeletedObject,
-    DeleteMarkerEntry,
-    DeleteObjectOutput,
-    DeleteObjectsOutput,
-    Delimiter,
-    EncodingType,
-    Error,
-    FetchOwner,
-    GetBucketLocationOutput,
-    GetObjectAttributesOutput,
-    GetObjectAttributesParts,
-    GetObjectAttributesRequest,
-    GetObjectOutput,
-    GetObjectRequest,
-    HeadBucketOutput,
-    HeadObjectOutput,
-    HeadObjectRequest,
-    InvalidArgument,
-    InvalidBucketName,
-    InvalidObjectState,
-    InvalidStorageClass,
-    KeyMarker,
-    ListBucketsOutput,
-    ListObjectsOutput,
-    ListObjectsV2Output,
-    ListObjectVersionsOutput,
-    Marker,
-    MaxKeys,
-    NoSuchBucket,
-    Object,
-    ObjectIdentifier,
-    ObjectKey,
-    ObjectVersion,
-    ObjectVersionId,
-    ObjectVersionStorageClass,
-    OptionalObjectAttributesList,
-    Prefix,
-    PutObjectOutput,
-    PutObjectRequest,
-    RequestPayer,
-    RestoreObjectOutput,
-    RestoreRequest,
-    S3Api,
-    ServerSideEncryption,
-    StartAfter,
-    StorageClass,
-    Token,
-    VersionIdMarker,
+from botocore.utils import InvalidArnException
+from moto.core.utils import camelcase_to_pascal, underscores_to_camelcase
+from moto.sns import sns_backends
+from moto.sns.models import MAXIMUM_MESSAGE_LENGTH, SNSBackend, Topic
+from moto.sns.utils import is_e164
+
+from localstack.aws.accounts import get_aws_account_id
+from localstack.aws.api import CommonServiceException, RequestContext
+from localstack.aws.api.sns import (
+    AmazonResourceName,
+    BatchEntryIdsNotDistinctException,
+    ConfirmSubscriptionResponse,
+    CreateEndpointResponse,
+    CreatePlatformApplicationResponse,
+    CreateTopicResponse,
+    GetSubscriptionAttributesResponse,
+    GetTopicAttributesResponse,
+    InvalidParameterException,
+    InvalidParameterValueException,
+    ListTagsForResourceResponse,
+    MapStringToString,
+    MessageAttributeMap,
+    NotFoundException,
+    PublishBatchRequestEntryList,
+    PublishBatchResponse,
+    PublishBatchResultEntry,
+    PublishResponse,
+    SnsApi,
+    String,
+    SubscribeResponse,
+    SubscriptionAttributesMap,
+    TagKeyList,
+    TagList,
+    TagResourceResponse,
+    TooManyEntriesInBatchRequestException,
+    TopicAttributesMap,
+    UntagResourceResponse,
+    attributeName,
+    attributeValue,
+    authenticateOnUnsubscribe,
+    boolean,
+    messageStructure,
+    subscriptionARN,
+    topicARN,
+    topicName,
 )
+from localstack.http import Request, Response, Router, route
+from localstack.services.edge import ROUTER
+from localstack.services.moto import call_moto
 from localstack.services.plugins import ServiceLifecycleHook
-from localstack.services.s3.codec import AwsChunkedDecoder
-from localstack.services.s3.constants import ARCHIVES_STORAGE_CLASSES
-from localstack.services.s3.exceptions import (
-    InvalidLocationConstraint,
-    InvalidRequest,
-    MalformedXML,
+from localstack.services.sns import constants as sns_constants
+from localstack.services.sns.models import SnsMessage, SnsStore, sns_stores
+from localstack.services.sns.publisher import (
+    PublishDispatcher,
+    SnsBatchPublishContext,
+    SnsPublishContext,
 )
-from localstack.services.s3.utils import (
-    add_expiration_days_to_datetime,
-    extract_bucket_key_version_id_from_copy_source,
-    get_class_attrs_from_spec_class,
-    get_full_default_bucket_location,
-    get_owner_for_account_id,
-    get_system_metadata_from_request,
-    is_bucket_name_valid,
-    parse_range_header,
-    validate_kms_key_id,
-)
-from localstack.services.s3.v3.models import S3Bucket, S3DeleteMarker, S3Object, S3Store, s3_stores
-from localstack.services.s3.v3.storage.core import LimitedIterableStream
-from localstack.services.s3.v3.storage.ephemeral import EphemeralS3ObjectStore
-from localstack.utils.strings import to_str
+from localstack.utils.aws.arns import ArnData, parse_arn
+from localstack.utils.strings import short_uid
 
+# set up logger
 LOG = logging.getLogger(__name__)
 
-STORAGE_CLASSES = get_class_attrs_from_spec_class(StorageClass)
-
-# TODO: pre-signed URLS -> REMAP parameters from querystring to headers???
-#  create a handler which handle pre-signed and remap before parsing the request!
 
+class SnsProvider(SnsApi, ServiceLifecycleHook):
+    """
+    Provider class for AWS Simple Notification Service.
+
+    AWS supports following operations in a cross-account setup:
+    - GetTopicAttributes
+    - SetTopicAttributes
+    - AddPermission
+    - RemovePermission
+    - Publish
+    - Subscribe
+    - ListSubscriptionByTopic
+    - DeleteTopic
+    """
 
-class S3Provider(S3Api, ServiceLifecycleHook):
     def __init__(self) -> None:
         super().__init__()
-        self._storage_backend = EphemeralS3ObjectStore()
-
-    @staticmethod
-    def get_store(account_id: str, region_name: str) -> S3Store:
-        # Use default account id for external access? would need an anonymous one
-        return s3_stores[account_id][region_name]
-
-    @handler("CreateBucket", expand=False)
-    def create_bucket(
-        self,
-        context: RequestContext,
-        request: CreateBucketRequest,
-    ) -> CreateBucketOutput:
-        bucket_name = request["Bucket"]
-
-        if not is_bucket_name_valid(bucket_name):
-            raise InvalidBucketName("The specified bucket is not valid.", BucketName=bucket_name)
-        if create_bucket_configuration := request.get("CreateBucketConfiguration"):
-            if not (bucket_region := create_bucket_configuration.get("LocationConstraint")):
-                raise MalformedXML()
-
-            if bucket_region == "us-east-1":
-                raise InvalidLocationConstraint("The specified location-constraint is not valid")
-        else:
-            bucket_region = "us-east-1"
-            if context.region != bucket_region:
-                raise CommonServiceException(
-                    code="IllegalLocationConstraintException",
-                    message="The unspecified location constraint is incompatible for the region specific endpoint this request was sent to.",
-                )
+        self._publisher = PublishDispatcher()
 
-        store = self.get_store(context.account_id, bucket_region)
+    def on_before_stop(self):
+        self._publisher.shutdown()
 
-        if bucket_name in store.global_bucket_map:
-            existing_bucket_owner = store.global_bucket_map[bucket_name]
-            if existing_bucket_owner != context.account_id:
-                raise BucketAlreadyExists()
-
-            # if the existing bucket has the same owner, the behaviour will depend on the region
-            if bucket_region != "us-east-1":
-                raise BucketAlreadyOwnedByYou()
-
-        s3_bucket = S3Bucket(
-            name=bucket_name,
-            account_id=context.account_id,
-            bucket_region=bucket_region,
-            acl=None,  # TODO: validate ACL first, create utils for validating and consolidating
-            object_ownership=request.get("ObjectOwnership"),
-            object_lock_enabled_for_bucket=request.get("ObjectLockEnabledForBucket"),
-        )
-        store.buckets[bucket_name] = s3_bucket
-        store.global_bucket_map[bucket_name] = s3_bucket.bucket_account_id
+    def on_after_init(self):
+        # Allow sent platform endpoint messages to be retrieved from the SNS endpoint
+        register_sns_api_resource(ROUTER)
 
-        # Location is always contained in response -> full url for LocationConstraint outside us-east-1
-        location = (
-            f"/{bucket_name}"
-            if bucket_region == "us-east-1"
-            else get_full_default_bucket_location(bucket_name)
-        )
-        response = CreateBucketOutput(Location=location)
-        return response
+    @staticmethod
+    def get_store(account_id: str, region_name: str) -> SnsStore:
+        return sns_stores[account_id][region_name]
 
-    def delete_bucket(
-        self, context: RequestContext, bucket: BucketName, expected_bucket_owner: AccountId = None
-    ) -> None:
-        store = self.get_store(context.account_id, context.region)
-        if not (s3_bucket := store.buckets.get(bucket)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket)
+    @staticmethod
+    def get_moto_backend(account_id: str, region_name: str) -> SNSBackend:
+        return sns_backends[account_id][region_name]
 
-        # the bucket still contains objects
-        if not s3_bucket.objects.is_empty():
-            raise BucketNotEmpty(
-                message="The bucket you tried to delete is not empty",
-                BucketName=bucket,
+    @staticmethod
+    def _get_topic(arn: str, context: RequestContext) -> Topic:
+        arn_data = parse_and_validate_topic_arn(arn)
+        try:
+            return sns_backends[arn_data["account"]][context.region].topics[arn]
+        except KeyError:
+            raise NotFoundException("Topic does not exist")
+
+    def get_topic_attributes(
+        self, context: RequestContext, topic_arn: topicARN
+    ) -> GetTopicAttributesResponse:
+        moto_response: GetTopicAttributesResponse = call_moto(context)
+        # TODO: fix some attributes by moto, see snapshot
+        # DeliveryPolicy
+        # EffectiveDeliveryPolicy
+        # Policy.Statement..Action -> SNS:Receive is added by moto but not returned in AWS
+        # TODO: very hacky way to get the attributes we need instead of a moto patch
+        # see the attributes we need: https://docs.aws.amazon.com/sns/latest/dg/sns-topic-attributes.html
+        # would need more work to have the proper format out of moto, maybe extract the model to our store
+        moto_topic_model = self._get_topic(topic_arn, context)
+        for attr in vars(moto_topic_model):
+            if "success_feedback" in attr:
+                key = camelcase_to_pascal(underscores_to_camelcase(attr))
+                moto_response["Attributes"][key] = getattr(moto_topic_model, attr)
+            elif attr == "signature_version":
+                moto_response["Attributes"]["SignatureVersion"] = moto_topic_model.signature_version
+        return moto_response
+
+    def publish_batch(
+        self,
+        context: RequestContext,
+        topic_arn: topicARN,
+        publish_batch_request_entries: PublishBatchRequestEntryList,
+    ) -> PublishBatchResponse:
+        if len(publish_batch_request_entries) > 10:
+            raise TooManyEntriesInBatchRequestException(
+                "The batch request contains more entries than permissible."
             )
 
-        store.buckets.pop(bucket)
-        store.global_bucket_map.pop(bucket)
-
-    def list_buckets(
-        self,
-        context: RequestContext,
-    ) -> ListBucketsOutput:
-        owner = get_owner_for_account_id(context.account_id)
-        store = self.get_store(context.account_id, context.region)
-        buckets = [
-            Bucket(Name=bucket.name, CreationDate=bucket.creation_date)
-            for bucket in store.buckets.values()
-        ]
-        return ListBucketsOutput(Owner=owner, Buckets=buckets)
-
-    def head_bucket(
-        self, context: RequestContext, bucket: BucketName, expected_bucket_owner: AccountId = None
-    ) -> HeadBucketOutput:
-        store = self.get_store(context.account_id, context.region)
-        if not (s3_bucket := store.buckets.get(bucket)):
-            # just to return the 404 error message
-            raise NoSuchBucket()
-
-        # TODO: this call is also used to check if the user has access/authorization for the bucket
-        #  it can return 403
-        return HeadBucketOutput(BucketRegion=s3_bucket.bucket_region)
-
-    def get_bucket_location(
-        self, context: RequestContext, bucket: BucketName, expected_bucket_owner: AccountId = None
-    ) -> GetBucketLocationOutput:
-        """
-        When implementing the ASF provider, this operation is implemented because:
-        - The spec defines a root element GetBucketLocationOutput containing a LocationConstraint member, where
-          S3 actually just returns the LocationConstraint on the root level (only operation so far that we know of).
-        - We circumvent the root level element here by patching the spec such that this operation returns a
-          single "payload" (the XML body response), which causes the serializer to directly take the payload element.
-        - The above "hack" causes the fix in the serializer to not be picked up here as we're passing the XML body as
-          the payload, which is why we need to manually do this here by manipulating the string.
-        Botocore implements this hack for parsing the response in `botocore.handlers.py#parse_get_bucket_location`
-        """
-        store = self.get_store(context.account_id, context.region)
-        if not (s3_bucket := store.buckets.get(bucket)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket)
-
-        location_constraint = (
-            '<?xml version="1.0" encoding="UTF-8"?>\n'
-            '<LocationConstraint xmlns="http://s3.amazonaws.com/doc/2006-03-01/">{{location}}</LocationConstraint>'
-        )
-
-        location = s3_bucket.bucket_region if s3_bucket.bucket_region != "us-east-1" else ""
-        location_constraint = location_constraint.replace("{{location}}", location)
-
-        response = GetBucketLocationOutput(LocationConstraint=location_constraint)
-        return response
-
-    @handler("PutObject", expand=False)
-    def put_object(
-        self,
-        context: RequestContext,
-        request: PutObjectRequest,
-    ) -> PutObjectOutput:
-        # TODO: validate order of validation
-        # TODO: still need to handle following parameters:
-        #  acl: ObjectCannedACL = None,
-        #  grant_full_control: GrantFullControl = None,
-        #  grant_read: GrantRead = None,
-        #  grant_read_acp: GrantReadACP = None,
-        #  grant_write_acp: GrantWriteACP = None,
-        #  -
-        #  request_payer: RequestPayer = None,
-        #  tagging: TaggingHeader = None,
-        #  object_lock_mode: ObjectLockMode = None,
-        #  object_lock_retain_until_date: ObjectLockRetainUntilDate = None,
-        #  object_lock_legal_hold_status: ObjectLockLegalHoldStatus = None,
-        store = self.get_store(context.account_id, context.region)
-        bucket_name = request["Bucket"]
-        if not (s3_bucket := store.buckets.get(bucket_name)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket_name)
-
-        if (
-            storage_class := request.get("StorageClass")
-        ) is not None and storage_class not in STORAGE_CLASSES:
-            raise InvalidStorageClass(
-                "The storage class you specified is not valid", StorageClassRequested=storage_class
+        parsed_arn = parse_and_validate_topic_arn(topic_arn)
+        store = self.get_store(account_id=parsed_arn["account"], region_name=context.region)
+        if topic_arn not in store.topic_subscriptions:
+            raise NotFoundException(
+                "Topic does not exist",
             )
 
-        if not config.S3_SKIP_KMS_KEY_VALIDATION and (sse_kms_key_id := request.get("SSEKMSKeyId")):
-            validate_kms_key_id(sse_kms_key_id, s3_bucket)
-
-        key = request["Key"]
-
-        system_metadata = get_system_metadata_from_request(request)
-        if not system_metadata.get("ContentType"):
-            system_metadata["ContentType"] = "binary/octet-stream"
-
-        # TODO: get all default from bucket once it is implemented
-        # validate encryption values
-
-        body = request.get("Body")
-        # check if chunked request
-        headers = context.request.headers
-        is_aws_chunked = headers.get("x-amz-content-sha256", "").startswith("STREAMING-")
-        if is_aws_chunked:
-            decoded_content_length = int(headers.get("x-amz-decoded-content-length", 0))
-            body = AwsChunkedDecoder(body, decoded_content_length)
-
-        # TODO check if key already exist, and if it is locked with LegalHold? so we don't override it if protected
-
-        version_id = generate_version_id(s3_bucket.versioning_status)
-
-        checksum_algorithm = request.get("ChecksumAlgorithm")
-        checksum_value = (
-            request.get(f"Checksum{checksum_algorithm.upper()}") if checksum_algorithm else None
-        )
-
-        s3_object = S3Object(
-            key=key,
-            version_id=version_id,
-            storage_class=storage_class,
-            expires=request.get("Expires"),
-            user_metadata=request.get("Metadata"),
-            system_metadata=system_metadata,
-            checksum_algorithm=checksum_algorithm,
-            checksum_value=checksum_value,
-            encryption=request.get("ServerSideEncryption"),
-            kms_key_id=request.get("SSEKMSKeyId"),
-            bucket_key_enabled=request.get("BucketKeyEnabled"),
-            lock_mode=request.get("ObjectLockMode"),
-            lock_legal_status=request.get("ObjectLockLegalHoldStatus"),
-            lock_until=request.get("ObjectLockRetainUntilDate"),
-            website_redirect_location=request.get("WebsiteRedirectLocation"),
-            expiration=None,  # TODO, from lifecycle, or should it be updated with config?
-            acl=None,
-        )
-
-        s3_stored_object = self._storage_backend.open(bucket_name, s3_object)
-        s3_stored_object.write(body)
-
-        if checksum_algorithm and s3_object.checksum_value != s3_stored_object.checksum():
-            self._storage_backend.remove(bucket_name, s3_object)
-            raise InvalidRequest(
-                f"Value for x-amz-checksum-{checksum_algorithm.lower()} header is invalid."
+        ids = [entry["Id"] for entry in publish_batch_request_entries]
+        if len(set(ids)) != len(publish_batch_request_entries):
+            raise BatchEntryIdsNotDistinctException(
+                "Two or more batch entries in the request have the same Id."
             )
 
-        s3_bucket.objects.set(key, s3_object)
-
-        # TODO: tags: do we have tagging service or do we manually handle? see utils TaggingService
+        response: PublishBatchResponse = {"Successful": [], "Failed": []}
 
-        # TODO: returned fields
-        # RequestCharged: Optional[RequestCharged]  # TODO
-        response = PutObjectOutput(
-            ETag=s3_object.quoted_etag,
-        )
-        if s3_object.version_id:  # TODO: better way?
-            response["VersionId"] = s3_object.version_id
-
-        if s3_object.checksum_algorithm:
-            response[f"Checksum{checksum_algorithm.upper()}"] = s3_object.checksum_value
-
-        if s3_object.expiration:
-            response["Expiration"] = s3_object.expiration  # TODO: properly parse the datetime
-
-        add_encryption_to_response(response, s3_object=s3_object)
-
-        return response
-
-    @handler("GetObject", expand=False)
-    def get_object(
-        self,
-        context: RequestContext,
-        request: GetObjectRequest,
-    ) -> GetObjectOutput:
-        # TODO: missing handling parameters:
-        #  if_match: IfMatch = None,
-        #  if_modified_since: IfModifiedSince = None,
-        #  if_none_match: IfNoneMatch = None,
-        #  if_unmodified_since: IfUnmodifiedSince = None,
-        #  response_cache_control: ResponseCacheControl = None,
-        #  response_content_disposition: ResponseContentDisposition = None,
-        #  response_content_encoding: ResponseContentEncoding = None,
-        #  response_content_language: ResponseContentLanguage = None,
-        #  response_content_type: ResponseContentType = None,
-        #  response_expires: ResponseExpires = None,
-        #  request_payer: RequestPayer = None,
-        #  part_number: PartNumber = None,
-        #  expected_bucket_owner: AccountId = None,
-
-        store = self.get_store(context.account_id, context.region)
-        bucket_name = request["Bucket"]
-        object_key = request["Key"]
-        if not (s3_bucket := store.buckets.get(bucket_name)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket_name)
-
-        # TODO implement PartNumber once multipart is done (being able to select only a Part)
-
-        s3_object = s3_bucket.get_object(
-            key=object_key,
-            version_id=request.get("VersionId"),
-            http_method="GET",
-        )
-
-        response = GetObjectOutput(
-            AcceptRanges="bytes",
-            **s3_object.get_system_metadata_fields(),
-        )
-        if s3_object.user_metadata:
-            response["Metadata"] = s3_object.user_metadata
-
-        if s3_object.parts and request.get("PartNumber"):
-            response["PartsCount"] = len(s3_object.parts)
-
-        if s3_object.version_id:
-            response["VersionId"] = s3_object.version_id
-
-        if s3_object.website_redirect_location:
-            response["WebsiteRedirectLocation"] = s3_object.website_redirect_location
-
-        if checksum_algorithm := s3_object.checksum_algorithm:
-            # this is a bug in AWS: it sets the content encoding header to an empty string (parity tested)
-            response["ContentEncoding"] = ""
-            if request.get("ChecksumMode", "").upper() == "ENABLED":
-                response[f"Checksum{checksum_algorithm.upper()}"] = s3_object.checksum_value
-
-        s3_stored_object = self._storage_backend.open(bucket_name, s3_object)
-
-        if range_header := request.get("Range"):
-            range_data = parse_range_header(range_header, s3_object.size)
-            s3_stored_object.seek(range_data.begin)
-            response["Body"] = LimitedIterableStream(
-                s3_stored_object, max_length=range_data.content_length
-            )
-            response["ContentRange"] = range_data.content_range
-            response["ContentLength"] = range_data.content_length
-            response["StatusCode"] = 206
-        else:
-            response["Body"] = s3_stored_object
-
-        # TODO: missing returned fields
-        #     Expiration: Optional[Expiration]
-        #     Restore: Optional[Restore]
-        #     RequestCharged: Optional[RequestCharged]
-        #     ReplicationStatus: Optional[ReplicationStatus]
-        #     TagCount: Optional[TagCount]
-        #     ObjectLockMode: Optional[ObjectLockMode]
-        #     ObjectLockRetainUntilDate: Optional[ObjectLockRetainUntilDate]
-        #     ObjectLockLegalHoldStatus: Optional[ObjectLockLegalHoldStatus]
+        # TODO: write AWS validated tests with FilterPolicy and batching
+        # TODO: find a scenario where we can fail to send a message synchronously to be able to report it
+        # right now, it seems that AWS fails the whole publish if something is wrong in the format of 1 message
+
+        message_contexts = []
+        for entry in publish_batch_request_entries:
+            message_attributes = entry.get("MessageAttributes", {})
+            if message_attributes:
+                # if a message contains non-valid message attributes
+                # will fail for the first non-valid message encountered, and raise ParameterValueInvalid
+                validate_message_attributes(message_attributes)
+
+            # TODO: WRITE AWS VALIDATED
+            if entry.get("MessageStructure") == "json":
+                try:
+                    message = json.loads(entry.get("Message"))
+                    # Keys in the JSON object that correspond to supported transport protocols must have
+                    # simple JSON string values.
+                    # Non-string values will cause the key to be ignored.
+                    message = {
+                        key: field for key, field in message.items() if isinstance(field, str)
+                    }
+                    if "default" not in message:
+                        raise InvalidParameterException(
+                            "Invalid parameter: Message Structure - No default entry in JSON message body"
+                        )
+                    entry["Message"] = message  # noqa
+                except json.JSONDecodeError:
+                    raise InvalidParameterException(
+                        "Invalid parameter: Message Structure - JSON message body failed to parse"
+                    )
 
-        return response
+            if is_fifo := (".fifo" in topic_arn):
+                if not all(["MessageGroupId" in entry for entry in publish_batch_request_entries]):
+                    raise InvalidParameterException(
+                        "Invalid parameter: The MessageGroupId parameter is required for FIFO topics"
+                    )
+                topic = self._get_topic(topic_arn, context)
+                if topic.content_based_deduplication == "false":
+                    if not all(
+                        [
+                            "MessageDeduplicationId" in entry
+                            for entry in publish_batch_request_entries
+                        ]
+                    ):
+                        raise InvalidParameterException(
+                            "Invalid parameter: The topic should either have ContentBasedDeduplication enabled or MessageDeduplicationId provided explicitly",
+                        )
 
-    @handler("HeadObject", expand=False)
-    def head_object(
-        self,
-        context: RequestContext,
-        request: HeadObjectRequest,
-    ) -> HeadObjectOutput:
-        store = self.get_store(context.account_id, context.region)
-        bucket_name = request["Bucket"]
-        object_key = request["Key"]
-        if not (s3_bucket := store.buckets.get(bucket_name)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket_name)
-
-        # TODO implement PartNumber, don't know about part number + version id?
-        #  if_match: IfMatch = None,
-        #  if_modified_since: IfModifiedSince = None,
-        #  if_none_match: IfNoneMatch = None,
-        #  if_unmodified_since: IfUnmodifiedSince = None,
-
-        s3_object = s3_bucket.get_object(
-            key=object_key,
-            version_id=request.get("VersionId"),
-            http_method="HEAD",
-        )
+            msg_ctx = SnsMessage.from_batch_entry(entry, is_fifo=is_fifo)
+            message_contexts.append(msg_ctx)
+            success = PublishBatchResultEntry(
+                Id=entry["Id"],
+                MessageId=msg_ctx.message_id,
+            )
+            if is_fifo:
+                success["SequenceNumber"] = msg_ctx.sequencer_number
+            response["Successful"].append(success)
 
-        response = HeadObjectOutput(
-            AcceptRanges="bytes",
-            **s3_object.get_system_metadata_fields(),
+        publish_ctx = SnsBatchPublishContext(
+            messages=message_contexts,
+            store=store,
+            request_headers=context.request.headers,
         )
-        if s3_object.user_metadata:
-            response["Metadata"] = s3_object.user_metadata
-
-        # TODO implements if_match if_modified_since if_none_match if_unmodified_since
-        if checksum_algorithm := s3_object.checksum_algorithm:
-            # this is a bug in AWS: it sets the content encoding header to an empty string (parity tested)
-            response["ContentEncoding"] = ""
-            if request.get("ChecksumMode", "").upper() == "ENABLED":
-                response[f"Checksum{checksum_algorithm.upper()}"] = checksum  # noqa
-
-        if range_header := request.get("Range"):
-            range_data = parse_range_header(range_header, s3_object.size)
-            response["ContentLength"] = range_data.content_length
-
-        if s3_object.parts:
-            response["PartsCount"] = len(s3_object.parts)
-
-        if s3_object.version_id:
-            response["VersionId"] = s3_object.version_id
-
-        if s3_object.website_redirect_location:
-            response["WebsiteRedirectLocation"] = s3_object.website_redirect_location
-
-        # TODO: missing return fields:
-        # Expiration: Optional[Expiration]
-        # Restore: Optional[Restore]
-        # ArchiveStatus: Optional[ArchiveStatus]
-
-        # RequestCharged: Optional[RequestCharged]
-        # ReplicationStatus: Optional[ReplicationStatus]
-        # ObjectLockMode: Optional[ObjectLockMode]
-        # ObjectLockRetainUntilDate: Optional[ObjectLockRetainUntilDate]
-        # ObjectLockLegalHoldStatus: Optional[ObjectLockLegalHoldStatus]
+        self._publisher.publish_batch_to_topic(publish_ctx, topic_arn)
 
         return response
 
-    def delete_object(
+    def set_subscription_attributes(
         self,
         context: RequestContext,
-        bucket: BucketName,
-        key: ObjectKey,
-        mfa: MFA = None,
-        version_id: ObjectVersionId = None,
-        request_payer: RequestPayer = None,
-        bypass_governance_retention: BypassGovernanceRetention = None,
-        expected_bucket_owner: AccountId = None,
-    ) -> DeleteObjectOutput:
-        # TODO: implement bypass_governance_retention, it is done in moto
-        store = self.get_store(context.account_id, context.region)
-        if not (s3_bucket := store.buckets.get(bucket)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket)
+        subscription_arn: subscriptionARN,
+        attribute_name: attributeName,
+        attribute_value: attributeValue = None,
+    ) -> None:
+        store = self.get_store(account_id=context.account_id, region_name=context.region)
+        sub = store.subscriptions.get(subscription_arn)
+        if not sub:
+            raise NotFoundException("Subscription does not exist")
+
+        validate_subscription_attribute(
+            attribute_name=attribute_name,
+            attribute_value=attribute_value,
+            topic_arn=sub["TopicArn"],
+        )
+        try:
+            call_moto(context)
+        except CommonServiceException as e:
+            # Moto errors don't send the "Type": "Sender" field in their SNS exception
+            if e.code == "InvalidParameter":
+                raise InvalidParameterException(e.message)
+            raise
 
-        if s3_bucket.versioning_status is None:
-            if version_id and version_id != "null":
-                raise InvalidArgument(
-                    "Invalid version id specified",
-                    ArgumentName="versionId",
-                    ArgumentValue=version_id,
-                )
+        if attribute_name == "FilterPolicy":
+            store = self.get_store(account_id=context.account_id, region_name=context.region)
+            store.subscription_filter_policy[subscription_arn] = json.loads(attribute_value)
+
+        sub[attribute_name] = attribute_value
+
+    def confirm_subscription(
+        self,
+        context: RequestContext,
+        topic_arn: topicARN,
+        token: String,
+        authenticate_on_unsubscribe: authenticateOnUnsubscribe = None,
+    ) -> ConfirmSubscriptionResponse:
+        # TODO: validate format on the token (seems to be 288 hex chars)
+        # this request can come from any http client, it might not be signed (we would need to implement
+        # `authenticate_on_unsubscribe` to force a signing client to do this request.
+        # so, the region and account_id might not be in the request. Use the ones from the topic_arn
+        try:
+            parsed_arn = parse_arn(topic_arn)
+        except InvalidArnException:
+            raise InvalidParameterException("Invalid parameter: Topic")
+
+        store = self.get_store(account_id=parsed_arn["account"], region_name=parsed_arn["region"])
+
+        # it seems SNS is able to know what the region of the topic should be, even though a wrong topic is accepted
+        if parsed_arn["region"] != get_region_from_subscription_token(token):
+            raise InvalidParameterException("Invalid parameter: Topic")
+
+        subscription_arn = store.subscription_tokens.get(token)
+        if not subscription_arn:
+            raise InvalidParameterException("Invalid parameter: Token")
+
+        subscription = store.subscriptions.get(subscription_arn)
+        if not subscription:
+            # subscription could have been deleted in the meantime
+            raise InvalidParameterException("Invalid parameter: Token")
+
+        # ConfirmSubscription is idempotent
+        if subscription.get("PendingConfirmation") == "false":
+            return ConfirmSubscriptionResponse(SubscriptionArn=subscription_arn)
+
+        subscription["PendingConfirmation"] = "false"
+        subscription["ConfirmationWasAuthenticated"] = "true"
+
+        return ConfirmSubscriptionResponse(SubscriptionArn=subscription_arn)
+
+    def untag_resource(
+        self, context: RequestContext, resource_arn: AmazonResourceName, tag_keys: TagKeyList
+    ) -> UntagResourceResponse:
+        call_moto(context)
+        # TODO: probably get the account_id and region from the `resource_arn`
+        store = self.get_store(context.account_id, context.region)
+        existing_tags = store.sns_tags.setdefault(resource_arn, [])
+        store.sns_tags[resource_arn] = [t for t in existing_tags if t["Key"] not in tag_keys]
+        return UntagResourceResponse()
+
+    def list_tags_for_resource(
+        self, context: RequestContext, resource_arn: AmazonResourceName
+    ) -> ListTagsForResourceResponse:
+        # TODO: probably get the account_id and region from the `resource_arn`
+        store = self.get_store(context.account_id, context.region)
+        tags = store.sns_tags.setdefault(resource_arn, [])
+        return ListTagsForResourceResponse(Tags=tags)
+
+    def create_platform_application(
+        self, context: RequestContext, name: String, platform: String, attributes: MapStringToString
+    ) -> CreatePlatformApplicationResponse:
+        # TODO: validate platform
+        # see https://docs.aws.amazon.com/cli/latest/reference/sns/create-platform-application.html
+        # list of possible values: ADM, Baidu, APNS, APNS_SANDBOX, GCM, MPNS, WNS
+        # each platform has a specific way to handle credentials
+        # this can also be used for dispatching message to the right platform
+        return call_moto(context)
+
+    def create_platform_endpoint(
+        self,
+        context: RequestContext,
+        platform_application_arn: String,
+        token: String,
+        custom_user_data: String = None,
+        attributes: MapStringToString = None,
+    ) -> CreateEndpointResponse:
+        # TODO: support mobile app events
+        # see https://docs.aws.amazon.com/sns/latest/dg/application-event-notifications.html
+        try:
+            result: CreateEndpointResponse = call_moto(context)
+        except CommonServiceException as e:
+            # TODO: this was unclear in the old provider, check against aws and moto
+            if "DuplicateEndpoint" in e.code:
+                moto_sns_backend = self.get_moto_backend(context.account_id, context.region)
+                for e in moto_sns_backend.platform_endpoints.values():
+                    if e.token == token:
+                        if custom_user_data and custom_user_data != e.custom_user_data:
+                            # TODO: check error against aws
+                            raise CommonServiceException(
+                                code="DuplicateEndpoint",
+                                message=f"Endpoint already exist for token: {token} with different attributes",
+                            )
+            raise
+        return result
 
-            found_object = s3_bucket.objects.pop(key, None)
-            # TODO: RequestCharged
-            if found_object:
-                self._storage_backend.remove(bucket, found_object)
-
-            return DeleteObjectOutput()
-
-        if not version_id:
-            delete_marker_id = generate_version_id(s3_bucket.versioning_status)
-            delete_marker = S3DeleteMarker(key=key, version_id=delete_marker_id)
-            # TODO: verify with Suspended bucket? does it override last version or still append?? big question
-            #  I think it puts a delete marker with a `null` VersionId, which deletes the object under
-            s3_bucket.objects.set(key, delete_marker)
-            return DeleteObjectOutput(VersionId=delete_marker.version_id, DeleteMarker=True)
-
-        if key not in s3_bucket.objects:
-            return DeleteObjectOutput()
-
-        if not (found_object := s3_bucket.objects.pop(object_key=key, version_id=version_id)):
-            raise InvalidArgument(
-                "Invalid version id specified",
-                ArgumentName="versionId",
-                ArgumentValue=version_id,
+    def unsubscribe(self, context: RequestContext, subscription_arn: subscriptionARN) -> None:
+        call_moto(context)
+        store = self.get_store(account_id=context.account_id, region_name=context.region)
+
+        # pop the subscription at the end, to avoid race condition by iterating over the topic subscriptions
+        subscription = store.subscriptions.get(subscription_arn)
+
+        if not subscription:
+            # unsubscribe is idempotent, so unsubscribing from a non-existing topic does nothing
+            return
+
+        if subscription["Protocol"] in ["http", "https"]:
+            # TODO: actually validate this (re)subscribe behaviour somehow (localhost.run?)
+            #  we might need to save the sub token in the store
+            subscription_token = encode_subscription_token_with_region(region=context.region)
+            message_ctx = SnsMessage(
+                type="UnsubscribeConfirmation",
+                token=subscription_token,
+                message=f"You have chosen to deactivate subscription {subscription_arn}.\nTo cancel this operation and restore the subscription, visit the SubscribeURL included in this message.",
+            )
+            publish_ctx = SnsPublishContext(
+                message=message_ctx, store=store, request_headers=context.request.headers
+            )
+            self._publisher.publish_to_topic_subscriber(
+                publish_ctx,
+                topic_arn=subscription["TopicArn"],
+                subscription_arn=subscription_arn,
             )
 
-        response = DeleteObjectOutput(VersionId=found_object.version_id)
-
-        if isinstance(found_object, S3DeleteMarker):
-            response["DeleteMarker"] = True
-        else:
-            self._storage_backend.remove(bucket, found_object)
-
-        return response
-
-    def delete_objects(
-        self,
-        context: RequestContext,
-        bucket: BucketName,
-        delete: Delete,
-        mfa: MFA = None,
-        request_payer: RequestPayer = None,
-        bypass_governance_retention: BypassGovernanceRetention = None,
-        expected_bucket_owner: AccountId = None,
-        checksum_algorithm: ChecksumAlgorithm = None,
-    ) -> DeleteObjectsOutput:
-        store = self.get_store(context.account_id, context.region)
-        if not (s3_bucket := store.buckets.get(bucket)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket)
+        store.topic_subscriptions[subscription["TopicArn"]].remove(subscription_arn)
+        store.subscription_filter_policy.pop(subscription_arn, None)
+        store.subscriptions.pop(subscription_arn, None)
+
+    def get_subscription_attributes(
+        self, context: RequestContext, subscription_arn: subscriptionARN
+    ) -> GetSubscriptionAttributesResponse:
+        store = self.get_store(account_id=context.account_id, region_name=context.region)
+        sub = store.subscriptions.get(subscription_arn)
+        if not sub:
+            raise NotFoundException("Subscription does not exist")
+        removed_attrs = ["sqs_queue_url"]
+        if "FilterPolicyScope" in sub and "FilterPolicy" not in sub:
+            removed_attrs.append("FilterPolicyScope")
+        elif "FilterPolicy" in sub and "FilterPolicyScope" not in sub:
+            sub["FilterPolicyScope"] = "MessageAttributes"
+
+        attributes = {k: v for k, v in sub.items() if k not in removed_attrs}
+        return GetSubscriptionAttributesResponse(Attributes=attributes)
+
+    def publish(
+        self,
+        context: RequestContext,
+        message: String,
+        topic_arn: topicARN = None,
+        target_arn: String = None,
+        phone_number: String = None,
+        subject: String = None,
+        message_structure: messageStructure = None,
+        message_attributes: MessageAttributeMap = None,
+        message_deduplication_id: String = None,
+        message_group_id: String = None,
+    ) -> PublishResponse:
+        if subject == "":
+            raise InvalidParameterException("Invalid parameter: Subject")
+        if not message or all(not m for m in message):
+            raise InvalidParameterException("Invalid parameter: Empty message")
+
+        # TODO: check for topic + target + phone number at the same time?
+        # TODO: more validation on phone, it might be opted out?
+        if phone_number and not is_e164(phone_number):
+            raise InvalidParameterException(
+                f"Invalid parameter: PhoneNumber Reason: {phone_number} is not valid to publish to"
+            )
 
-        objects: list[ObjectIdentifier] = delete.get("Objects")
-        if not objects:
-            raise MalformedXML()
-
-        # TODO: max 1000 delete at once? test against AWS?
-        # TODO: implement ByPassGovernance
-        # TODO: implement Locking error
-
-        quiet = delete.get("Quiet", False)
-        deleted = []
-        errors = []
-
-        to_remove = []
-        for to_delete_object in objects:
-            # TODO: beware of key encoding (XML?)
-            object_key = to_delete_object.get("Key")
-            version_id = to_delete_object.get("VersionId")
-            if s3_bucket.versioning_status is None:
-                if version_id and version_id != "null":
-                    errors.append(
-                        Error(
-                            Code="NoSuchVersion",
-                            Key=object_key,
-                            Message="The specified version does not exist.",
-                            VersionId=version_id,
-                        )
-                    )
-                    continue
+        if len(message) > MAXIMUM_MESSAGE_LENGTH:
+            raise InvalidParameterException("Invalid parameter: Message too long")
 
-                found_object = s3_bucket.objects.pop(object_key, None)
-                if found_object:
-                    to_remove.append(found_object)
-
-                if not quiet:
-                    deleted.append(DeletedObject(Key=object_key))
-
-                continue
-
-            if not version_id:
-                delete_marker_id = generate_version_id(s3_bucket.versioning_status)
-                delete_marker = S3DeleteMarker(key=object_key, version_id=delete_marker_id)
-                s3_bucket.objects.set(object_key, delete_marker)
-                if not quiet:
-                    deleted.append(
-                        DeletedObject(
-                            DeleteMarker=True,
-                            DeleteMarkerVersionId=delete_marker_id,
-                            Key=object_key,
-                        )
+        # for compatibility reasons, AWS allows users to use either TargetArn or TopicArn for publishing to a topic
+        # use any of them for topic validation
+        topic_or_target_arn = topic_arn or target_arn
+
+        if is_fifo := (topic_or_target_arn and ".fifo" in topic_or_target_arn):
+            if not message_group_id:
+                raise InvalidParameterException(
+                    "Invalid parameter: The MessageGroupId parameter is required for FIFO topics",
+                )
+            topic = self._get_topic(topic_or_target_arn, context)
+            if topic.content_based_deduplication == "false":
+                if not message_deduplication_id:
+                    raise InvalidParameterException(
+                        "Invalid parameter: The topic should either have ContentBasedDeduplication enabled or MessageDeduplicationId provided explicitly",
                     )
-                continue
-
-            if not (
-                found_object := s3_bucket.objects.pop(object_key=object_key, version_id=version_id)
-            ):
-                errors.append(
-                    Error(
-                        Code="NoSuchVersion",
-                        Key=object_key,
-                        Message="The specified version does not exist.",
-                        VersionId=version_id,
+        elif message_deduplication_id:
+            # this is the first one to raise if both are set while the topic is not fifo
+            raise InvalidParameterException(
+                "Invalid parameter: MessageDeduplicationId Reason: The request includes MessageDeduplicationId parameter that is not valid for this topic type"
+            )
+        elif message_group_id:
+            raise InvalidParameterException(
+                "Invalid parameter: MessageGroupId Reason: The request includes MessageGroupId parameter that is not valid for this topic type"
+            )
+        is_endpoint_publish = target_arn and ":endpoint/" in target_arn
+        if message_structure == "json":
+            try:
+                message = json.loads(message)
+                # Keys in the JSON object that correspond to supported transport protocols must have
+                # simple JSON string values.
+                # Non-string values will cause the key to be ignored.
+                message = {key: field for key, field in message.items() if isinstance(field, str)}
+                # TODO: check no default key for direct TargetArn endpoint publish, need credentials
+                # see example: https://docs.aws.amazon.com/sns/latest/dg/sns-send-custom-platform-specific-payloads-mobile-devices.html
+                if "default" not in message and not is_endpoint_publish:
+                    raise InvalidParameterException(
+                        "Invalid parameter: Message Structure - No default entry in JSON message body"
                     )
+            except json.JSONDecodeError:
+                raise InvalidParameterException(
+                    "Invalid parameter: Message Structure - JSON message body failed to parse"
                 )
-                continue
-
-            if not quiet:
-                deleted_object = DeletedObject(
-                    Key=object_key,
-                    VersionId=version_id,
-                )
-                if isinstance(found_object, S3DeleteMarker):
-                    deleted_object["DeleteMarker"] = True
-                    deleted_object["DeleteMarkerVersionId"] = found_object.version_id
-
-                deleted.append(deleted_object)
-
-            if isinstance(found_object, S3Object):
-                to_remove.append(found_object)
-
-        # TODO: request charged
-        self._storage_backend.remove(bucket, to_remove)
-        response: DeleteObjectsOutput = {}
-        # AWS validated: the list of Deleted objects is unordered, multiple identical calls can return different results
-        if errors:
-            response["Errors"] = errors
-        if not quiet:
-            response["Deleted"] = deleted
-
-        return response
-
-    @handler("CopyObject", expand=False)
-    def copy_object(
-        self,
-        context: RequestContext,
-        request: CopyObjectRequest,
-    ) -> CopyObjectOutput:
-        # TODO: handle those parameters next:
-        # acl: ObjectCannedACL = None,
-        # grant_full_control: GrantFullControl = None,
-        # grant_read: GrantRead = None,
-        # grant_read_acp: GrantReadACP = None,
-        # grant_write_acp: GrantWriteACP = None,
-        #
-        # copy_source_if_match: CopySourceIfMatch = None,
-        # copy_source_if_modified_since: CopySourceIfModifiedSince = None,
-        # copy_source_if_none_match: CopySourceIfNoneMatch = None,
-        # copy_source_if_unmodified_since: CopySourceIfUnmodifiedSince = None,
-        #
-        # tagging_directive: TaggingDirective = None,
-        # server_side_encryption: ServerSideEncryption = None,
-        # ssekms_key_id: SSEKMSKeyId = None,
-        # bucket_key_enabled: BucketKeyEnabled = None,
-        #
-        # request_payer: RequestPayer = None,
-        # tagging: TaggingHeader = None,
-        # object_lock_mode: ObjectLockMode = None,
-        # object_lock_retain_until_date: ObjectLockRetainUntilDate = None,
-        # object_lock_legal_hold_status: ObjectLockLegalHoldStatus = None,
-        dest_bucket = request["Bucket"]
-        dest_key = request["Key"]
-        store = self.get_store(context.account_id, context.region)
-        if not (dest_s3_bucket := store.buckets.get(dest_bucket)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=dest_bucket)
-
-        src_bucket, src_key, src_version_id = extract_bucket_key_version_id_from_copy_source(
-            request.get("CopySource")
-        )
-
-        if not (src_s3_bucket := store.buckets.get(src_bucket)):
-            # TODO: validate this
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=src_bucket)
-
-        # validate method not allowed?
-        # if the object is a delete marker, get_object will raise, like AWS
-        src_s3_object = src_s3_bucket.get_object(key=src_key, version_id=src_version_id)
 
-        # TODO: validate StorageClass for ARCHIVES one
-        if src_s3_object.storage_class in ARCHIVES_STORAGE_CLASSES:
-            raise
+        if message_attributes:
+            validate_message_attributes(message_attributes)
 
-        # TODO validate order of validation
-        storage_class = request.get("StorageClass")
-        server_side_encryption = request.get("ServerSideEncryption")
-        metadata_directive = request.get("MetadataDirective")
-        website_redirect_location = request.get("WebsiteRedirectLocation")
-        if src_key == dest_key and not any(
-            (
-                storage_class,
-                server_side_encryption,
-                metadata_directive == "REPLACE",
-                website_redirect_location,
-                dest_s3_bucket.encryption_rule,  # S3 will allow copy in place if the bucket has encryption configured
-            )
-        ):
-            raise InvalidRequest(
-                "This copy request is illegal because it is trying to copy an object to itself without changing the"
-                "object's metadata, storage class, website redirect location or encryption attributes."
-            )
-
-        if metadata_directive == "REPLACE":
-            user_metadata = request.get("Metadata")
-            system_metadata = get_system_metadata_from_request(request)
+        if not phone_number:
+            # use the account to get the store from the TopicArn (you can only publish in the same region as the topic)
+            parsed_arn = parse_and_validate_topic_arn(topic_or_target_arn)
+            store = self.get_store(account_id=parsed_arn["account"], region_name=context.region)
+            moto_sns_backend = self.get_moto_backend(parsed_arn["account"], context.region)
+            if is_endpoint_publish:
+                if target_arn not in moto_sns_backend.platform_endpoints:
+                    raise InvalidParameterException(
+                        "Invalid parameter: TargetArn Reason: No endpoint found for the target arn specified"
+                    )
+            else:
+                if topic_or_target_arn not in store.topic_subscriptions:
+                    raise NotFoundException(
+                        "Topic does not exist",
+                    )
         else:
-            user_metadata = src_s3_object.user_metadata
-            system_metadata = src_s3_object.system_metadata
-
-        dest_version_id = generate_version_id(dest_s3_bucket.versioning_status)
+            # use the store from the request context
+            store = self.get_store(account_id=context.account_id, region_name=context.region)
 
-        s3_object = S3Object(
-            key=dest_key,
-            etag=src_s3_object.etag,
-            size=src_s3_object.size,
-            version_id=dest_version_id,
-            storage_class=storage_class,
-            expires=request.get("Expires"),
-            user_metadata=user_metadata,
-            system_metadata=system_metadata,
-            checksum_algorithm=request.get("ChecksumAlgorithm") or src_s3_object.checksum_algorithm,
-            encryption=request.get("ServerSideEncryption"),
-            kms_key_id=request.get("SSEKMSKeyId"),
-            bucket_key_enabled=request.get("BucketKeyEnabled"),
-            lock_mode=request.get("ObjectLockMode"),
-            lock_legal_status=request.get("ObjectLockLegalHoldStatus"),
-            lock_until=request.get("ObjectLockRetainUntilDate"),
-            website_redirect_location=website_redirect_location,
-            expiration=None,  # TODO, from lifecycle
-            acl=None,
-        )
-
-        s3_stored_object = self._storage_backend.copy(
-            src_bucket=src_bucket,
-            src_object=src_s3_object,
-            dest_bucket=dest_bucket,
-            dest_object=s3_object,
-        )
-        s3_object.checksum_value = s3_stored_object.checksum() or s3_object.checksum_value
-
-        # Object copied from Glacier object should not have expiry
-        # TODO: verify this assumption from moto?
-        dest_s3_bucket.objects.set(dest_key, s3_object)
-
-        copy_object_result = CopyObjectResult(
-            ETag=s3_object.quoted_etag,
-            LastModified=s3_object.last_modified,
-        )
-        if s3_object.checksum_algorithm:
-            copy_object_result[
-                f"Checksum{s3_object.checksum_algorithm.upper()}"
-            ] = s3_object.checksum_value
-
-        response = CopyObjectOutput(
-            CopyObjectResult=copy_object_result,
-        )
-
-        if s3_object.version_id:
-            response["VersionId"] = s3_object.version_id
-
-        if s3_object.expiration:
-            response["Expiration"] = s3_object.expiration  # TODO: properly parse the datetime
-
-        add_encryption_to_response(response, s3_object=s3_object)
-
-        if src_version_id:
-            response["CopySourceVersionId"] = src_version_id
-
-        # RequestCharged: Optional[RequestCharged] # TODO
-
-        return response
-
-    def list_objects(
-        self,
-        context: RequestContext,
-        bucket: BucketName,
-        delimiter: Delimiter = None,
-        encoding_type: EncodingType = None,
-        marker: Marker = None,
-        max_keys: MaxKeys = None,
-        prefix: Prefix = None,
-        request_payer: RequestPayer = None,
-        expected_bucket_owner: AccountId = None,
-        optional_object_attributes: OptionalObjectAttributesList = None,
-    ) -> ListObjectsOutput:
-        store = self.get_store(context.account_id, context.region)
-        if not (s3_bucket := store.buckets.get(bucket)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket)
-
-        # TODO: URL encode keys (is it done already in serializer?)
-        common_prefixes = set()
-        count = 0
-        is_truncated = False
-        next_key_marker = None
-        max_keys = max_keys or 1000
-        prefix = prefix or ""
-
-        s3_objects: list[Object] = []
-
-        all_objects = s3_bucket.objects.values()
-        # sort by key
-        all_objects.sort(key=lambda r: r.key)
-
-        for s3_object in all_objects:
-            key = s3_object.key
-            # skip all keys that alphabetically come before key_marker
-            if marker:
-                if key <= marker:
-                    continue
-
-            # Filter for keys that start with prefix
-            if prefix and not key.startswith(prefix):
-                continue
-
-            # separate keys that contain the same string between the prefix and the first occurrence of the delimiter
-            if delimiter and delimiter in (key_no_prefix := key.removeprefix(prefix)):
-                pre_delimiter, _, _ = key_no_prefix.partition(delimiter)
-                prefix_including_delimiter = f"{prefix}{pre_delimiter}{delimiter}"
-
-                if prefix_including_delimiter not in common_prefixes:
-                    count += 1
-                    common_prefixes.add(prefix_including_delimiter)
-                continue
-
-            # TODO: add RestoreStatus if present
-            object_data = Object(
-                Key=s3_object.key,
-                ETag=s3_object.quoted_etag,
-                Owner=s3_bucket.owner,  # TODO: verify reality
-                Size=s3_object.size,
-                LastModified=s3_object.last_modified,
-                StorageClass=s3_object.storage_class,
-            )
-
-            if s3_object.checksum_algorithm:
-                object_data["ChecksumAlgorithm"] = [s3_object.checksum_algorithm]
-
-            s3_objects.append(object_data)
-
-            count += 1
-            if count >= max_keys:
-                is_truncated = True
-                next_key_marker = s3_object.key
-                break
-
-        common_prefixes = [CommonPrefix(Prefix=prefix) for prefix in sorted(common_prefixes)]
-
-        response = ListObjectsOutput(
-            IsTruncated=is_truncated,
-            Name=bucket,
-            MaxKeys=max_keys,
-            EncodingType=EncodingType.url,
-            Prefix=prefix or "",
-            Marker=marker or "",
-        )
-        if s3_objects:
-            response["Contents"] = s3_objects
-        if delimiter:
-            response["Delimiter"] = delimiter
-        if common_prefixes:
-            response["CommonPrefixes"] = common_prefixes
-        if delimiter and next_key_marker:
-            response["NextMarker"] = next_key_marker
+        message_ctx = SnsMessage(
+            type="Notification",
+            message=message,
+            message_attributes=message_attributes,
+            message_deduplication_id=message_deduplication_id,
+            message_group_id=message_group_id,
+            message_structure=message_structure,
+            subject=subject,
+            is_fifo=is_fifo,
+        )
+        publish_ctx = SnsPublishContext(
+            message=message_ctx, store=store, request_headers=context.request.headers
+        )
+
+        if is_endpoint_publish:
+            self._publisher.publish_to_application_endpoint(
+                ctx=publish_ctx, endpoint_arn=target_arn
+            )
+        elif phone_number:
+            self._publisher.publish_to_phone_number(ctx=publish_ctx, phone_number=phone_number)
+        else:
+            # beware if the subscription is FIFO, the order might not be guaranteed.
+            # 2 quick call to this method in succession might not be executed in order in the executor?
+            # TODO: test how this behaves in a FIFO context with a lot of threads.
+            self._publisher.publish_to_topic(publish_ctx, topic_or_target_arn)
+
+        if is_fifo:
+            return PublishResponse(
+                MessageId=message_ctx.message_id, SequenceNumber=message_ctx.sequencer_number
+            )
 
-        # RequestCharged: Optional[RequestCharged]  # TODO
-        return response
+        return PublishResponse(MessageId=message_ctx.message_id)
 
-    def list_objects_v2(
+    def subscribe(
         self,
         context: RequestContext,
-        bucket: BucketName,
-        delimiter: Delimiter = None,
-        encoding_type: EncodingType = None,
-        max_keys: MaxKeys = None,
-        prefix: Prefix = None,
-        continuation_token: Token = None,
-        fetch_owner: FetchOwner = None,
-        start_after: StartAfter = None,
-        request_payer: RequestPayer = None,
-        expected_bucket_owner: AccountId = None,
-        optional_object_attributes: OptionalObjectAttributesList = None,
-    ) -> ListObjectsV2Output:
-        store = self.get_store(context.account_id, context.region)
-        if not (s3_bucket := store.buckets.get(bucket)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket)
-
-        if continuation_token and continuation_token == "":
-            raise InvalidArgument("The continuation token provided is incorrect")
-
-        # TODO: URL encode keys (is it done already in serializer?)
-        common_prefixes = set()
-        count = 0
-        is_truncated = False
-        next_continuation_token = None
-        max_keys = max_keys or 1000
-        prefix = prefix or ""
-        decoded_continuation_token = (
-            to_str(base64.urlsafe_b64decode(continuation_token.encode()))
-            if continuation_token
-            else None
-        )
-
-        s3_objects: list[Object] = []
-
-        all_objects = s3_bucket.objects.values()
-        # sort by key
-        all_objects.sort(key=lambda r: r.key)
-
-        for s3_object in all_objects:
-            key = s3_object.key
-            # skip all keys that alphabetically come before key_marker
-            # TODO: what if there's StartAfter AND ContinuationToken
-            if continuation_token:
-                if key < decoded_continuation_token:
-                    continue
-
-            if start_after:
-                if key < start_after:
-                    continue
-
-            # Filter for keys that start with prefix
-            if prefix and not key.startswith(prefix):
-                continue
-
-            # separate keys that contain the same string between the prefix and the first occurrence of the delimiter
-            if delimiter and delimiter in (key_no_prefix := key.removeprefix(prefix)):
-                pre_delimiter, _, _ = key_no_prefix.partition(delimiter)
-                prefix_including_delimiter = f"{prefix}{pre_delimiter}{delimiter}"
-
-                if prefix_including_delimiter not in common_prefixes:
-                    count += 1
-                    common_prefixes.add(prefix_including_delimiter)
-                continue
-
-            count += 1
-            if count > max_keys:
-                is_truncated = True
-                next_continuation_token = to_str(base64.urlsafe_b64encode(s3_object.key.encode()))
-                break
-
-            # TODO: add RestoreStatus if present
-            object_data = Object(
-                Key=s3_object.key,
-                ETag=s3_object.quoted_etag,
-                Size=s3_object.size,
-                LastModified=s3_object.last_modified,
-                StorageClass=s3_object.storage_class,
-            )
-
-            if fetch_owner:
-                object_data["Owner"] = s3_bucket.owner
-
-            if s3_object.checksum_algorithm:
-                object_data["ChecksumAlgorithm"] = [s3_object.checksum_algorithm]
-
-            s3_objects.append(object_data)
-
-        common_prefixes = [CommonPrefix(Prefix=prefix) for prefix in sorted(common_prefixes)]
-
-        response = ListObjectsV2Output(
-            IsTruncated=is_truncated,
-            Name=bucket,
-            MaxKeys=max_keys,
-            EncodingType=EncodingType.url,
-            Prefix=prefix or "",
-            KeyCount=count,
-        )
-        if s3_objects:
-            response["Contents"] = s3_objects
-        if delimiter:
-            response["Delimiter"] = delimiter
-        if common_prefixes:
-            response["CommonPrefixes"] = common_prefixes
-        if next_continuation_token:
-            response["NextContinuationToken"] = next_continuation_token
-        if continuation_token:
-            response["ContinuationToken"] = continuation_token
-        if start_after:
-            response["StartAfter"] = start_after
-
-        # RequestCharged: Optional[RequestCharged]  # TODO
-        return response
+        topic_arn: topicARN,
+        protocol: String,
+        endpoint: String = None,
+        attributes: SubscriptionAttributesMap = None,
+        return_subscription_arn: boolean = None,
+    ) -> SubscribeResponse:
+        if not endpoint:
+            # TODO: check AWS behaviour (because endpoint is optional)
+            raise NotFoundException("Endpoint not specified in subscription")
+        if protocol not in sns_constants.SNS_PROTOCOLS:
+            raise InvalidParameterException(
+                f"Invalid parameter: Amazon SNS does not support this protocol string: {protocol}"
+            )
+        elif protocol in ["http", "https"] and not endpoint.startswith(f"{protocol}://"):
+            raise InvalidParameterException(
+                "Invalid parameter: Endpoint must match the specified protocol"
+            )
+        elif protocol == "sms" and not is_e164(endpoint):
+            raise InvalidParameterException(f"Invalid SMS endpoint: {endpoint}")
 
-    def list_object_versions(
-        self,
-        context: RequestContext,
-        bucket: BucketName,
-        delimiter: Delimiter = None,
-        encoding_type: EncodingType = None,
-        key_marker: KeyMarker = None,
-        max_keys: MaxKeys = None,
-        prefix: Prefix = None,
-        version_id_marker: VersionIdMarker = None,
-        expected_bucket_owner: AccountId = None,
-        request_payer: RequestPayer = None,
-        optional_object_attributes: OptionalObjectAttributesList = None,
-    ) -> ListObjectVersionsOutput:
-        store = self.get_store(context.account_id, context.region)
-        if not (s3_bucket := store.buckets.get(bucket)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket)
+        elif protocol == "sqs":
+            try:
+                parse_arn(endpoint)
+            except InvalidArnException:
+                raise InvalidParameterException("Invalid parameter: SQS endpoint ARN")
+
+        if ".fifo" in endpoint and ".fifo" not in topic_arn:
+            raise InvalidParameterException(
+                "Invalid parameter: Invalid parameter: Endpoint Reason: FIFO SQS Queues can not be subscribed to standard SNS topics"
+            )
+        elif ".fifo" in topic_arn and ".fifo" not in endpoint:
+            raise InvalidParameterException(
+                "Invalid parameter: Invalid parameter: Endpoint Reason: Please use FIFO SQS queue"
+            )
+        if attributes:
+            for attr_name, attr_value in attributes.items():
+                validate_subscription_attribute(
+                    attribute_name=attr_name, attribute_value=attr_value, topic_arn=topic_arn
+                )
 
-        # TODO: URL encode keys (is it done already in serializer?)
-        common_prefixes = set()
-        count = 0
-        is_truncated = False
-        next_key_marker = None
-        next_version_id_marker = None
-        max_keys = max_keys or 1000
-        prefix = prefix or ""
-
-        object_versions: list[ObjectVersion] = []
-        delete_markers: list[DeleteMarkerEntry] = []
-
-        all_versions = s3_bucket.objects.values(with_versions=True)
-        # sort by key, and last-modified-date, to get the last version first
-        all_versions.sort(key=lambda r: (r.key, -r.last_modified.timestamp()))
-
-        for version in all_versions:
-            key = version.key
-            # skip all keys that alphabetically come before key_marker
-            if key_marker:
-                if key < key_marker:
-                    continue
-                elif key == key_marker:
-                    # if we're at the key_marker, skip versions that are before version_id_marker
-                    if version_id_marker and version.version_id < version_id_marker:
-                        continue
-
-            # Filter for keys that start with prefix
-            if prefix and not key.startswith(prefix):
-                continue
-
-            # separate keys that contain the same string between the prefix and the first occurrence of the delimiter
-            if delimiter and delimiter in (key_no_prefix := key.removeprefix(prefix)):
-                pre_delimiter, _, _ = key_no_prefix.partition(delimiter)
-                prefix_including_delimiter = f"{prefix}{pre_delimiter}{delimiter}"
-
-                if prefix_including_delimiter not in common_prefixes:
-                    count += 1
-                    common_prefixes.add(prefix_including_delimiter)
-                continue
-
-            count += 1
-            if count > max_keys:
-                is_truncated = True
-                next_key_marker = version.key
-                next_version_id_marker = version.version_id
-                break
-
-            if isinstance(version, S3DeleteMarker):
-                delete_marker = DeleteMarkerEntry(
-                    Key=version.key,
-                    Owner=s3_bucket.owner,
-                    VersionId=version.version_id,
-                    IsLatest=version.is_current,
-                    LastModified=version.last_modified,
+        moto_response = call_moto(context)
+        subscription_arn = moto_response.get("SubscriptionArn")
+        parsed_topic_arn = parse_and_validate_topic_arn(topic_arn)
+
+        store = self.get_store(account_id=parsed_topic_arn["account"], region_name=context.region)
+
+        # An endpoint may only be subscribed to a topic once. Subsequent
+        # subscribe calls do nothing (subscribe is idempotent).
+        for existing_topic_subscription in store.topic_subscriptions.get(topic_arn, []):
+            sub = store.subscriptions.get(existing_topic_subscription, {})
+            if sub.get("Endpoint") == endpoint:
+                return SubscribeResponse(SubscriptionArn=sub["SubscriptionArn"])
+
+        subscription = {
+            # http://docs.aws.amazon.com/cli/latest/reference/sns/get-subscription-attributes.html
+            "TopicArn": topic_arn,
+            "Endpoint": endpoint,
+            "Protocol": protocol,
+            "SubscriptionArn": subscription_arn,
+            "PendingConfirmation": "true",
+            "Owner": context.account_id,
+            "RawMessageDelivery": "false",  # default value, will be overriden if set
+        }
+        if attributes:
+            subscription.update(attributes)
+            if "FilterPolicy" in attributes:
+                store.subscription_filter_policy[subscription_arn] = json.loads(
+                    attributes["FilterPolicy"]
                 )
-                delete_markers.append(delete_marker)
-                continue
 
-            # TODO: add RestoreStatus if present
-            object_version = ObjectVersion(
-                Key=version.key,
-                ETag=version.quoted_etag,
-                Owner=s3_bucket.owner,  # TODO: verify reality
-                Size=version.size,
-                VersionId=version.version_id or "null",
-                LastModified=version.last_modified,
-                IsLatest=version.is_current,
-                # TODO: verify this, are other class possible?
-                # StorageClass=version.storage_class,
-                StorageClass=ObjectVersionStorageClass.STANDARD,
-            )
-
-            if version.checksum_algorithm:
-                object_version["ChecksumAlgorithm"] = [version.checksum_algorithm]
-
-            object_versions.append(object_version)
-
-        common_prefixes = [CommonPrefix(Prefix=prefix) for prefix in sorted(common_prefixes)]
-
-        response = ListObjectVersionsOutput(
-            IsTruncated=is_truncated,
-            Name=bucket,
-            MaxKeys=max_keys,
-            EncodingType=EncodingType.url,
-            Prefix=prefix,
-            KeyMarker=key_marker or "",
-            VersionIdMarker=version_id_marker or "",
-        )
-        if object_versions:
-            response["Versions"] = object_versions
-        if delete_markers:
-            response["DeleteMarkers"] = delete_markers
-        if delimiter:
-            response["Delimiter"] = delimiter
-        if common_prefixes:
-            response["CommonPrefixes"] = common_prefixes
-        if next_key_marker:
-            response["NextKeyMarker"] = next_key_marker
-        if next_version_id_marker:
-            response["NextVersionIdMarker"] = next_version_id_marker
+        store.subscriptions[subscription_arn] = subscription
 
-        # RequestCharged: Optional[RequestCharged]  # TODO
-        return response
+        topic_subscription = store.topic_subscriptions.setdefault(topic_arn, [])
+        topic_subscription.append(subscription_arn)
 
-    @handler("GetObjectAttributes", expand=False)
-    def get_object_attributes(
-        self,
-        context: RequestContext,
-        request: GetObjectAttributesRequest,
-    ) -> GetObjectAttributesOutput:
-        store = self.get_store(context.account_id, context.region)
-        bucket_name = request["Bucket"]
-        object_key = request["Key"]
-        if not (s3_bucket := store.buckets.get(bucket_name)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket_name)
-
-        s3_object = s3_bucket.get_object(
-            key=object_key,
-            version_id=request.get("VersionId"),
-            http_method="GET",
-        )
+        # store the token and subscription arn
+        # TODO: the token is a 288 hex char string
+        subscription_token = encode_subscription_token_with_region(region=context.region)
+        store.subscription_tokens[subscription_token] = subscription_arn
+
+        # Send out confirmation message for HTTP(S), fix for https://github.com/localstack/localstack/issues/881
+        if protocol in ["http", "https"]:
+            message_ctx = SnsMessage(
+                type="SubscriptionConfirmation",
+                token=subscription_token,
+                message=f"You have chosen to subscribe to the topic {topic_arn}.\nTo confirm the subscription, visit the SubscribeURL included in this message.",
+            )
+            publish_ctx = SnsPublishContext(
+                message=message_ctx, store=store, request_headers=context.request.headers
+            )
+            self._publisher.publish_to_topic_subscriber(
+                ctx=publish_ctx,
+                topic_arn=topic_arn,
+                subscription_arn=subscription_arn,
+            )
+        elif protocol not in ["email", "email-json"]:
+            # Only HTTP(S) and email subscriptions are not auto validated
+            # Except if the endpoint and the topic are not in the same AWS account, then you'd need to manually confirm
+            # the subscription with the token
+            # TODO: revisit for multi-account
+            # TODO: test with AWS for email & email-json confirmation message
+            # we need to add the following check:
+            # if parsed_topic_arn["account"] == endpoint account (depending on the type, SQS, lambda, parse the arn)
+            subscription["PendingConfirmation"] = "false"
+            subscription["ConfirmationWasAuthenticated"] = "true"
+        return SubscribeResponse(SubscriptionArn=subscription_arn)
+
+    def tag_resource(
+        self, context: RequestContext, resource_arn: AmazonResourceName, tags: TagList
+    ) -> TagResourceResponse:
+        # each tag key must be unique
+        # https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html#tag-best-practices
+        unique_tag_keys = {tag["Key"] for tag in tags}
+        if len(unique_tag_keys) < len(tags):
+            raise InvalidParameterException("Invalid parameter: Duplicated keys are not allowed.")
+
+        call_moto(context)
+        store = self.get_store(context.account_id, context.region)
+        existing_tags = store.sns_tags.get(resource_arn, [])
+
+        def existing_tag_index(_item):
+            for idx, tag in enumerate(existing_tags):
+                if _item["Key"] == tag["Key"]:
+                    return idx
+            return None
+
+        for item in tags:
+            existing_index = existing_tag_index(item)
+            if existing_index is None:
+                existing_tags.append(item)
+            else:
+                existing_tags[existing_index] = item
+
+        store.sns_tags[resource_arn] = existing_tags
+        return TagResourceResponse()
+
+    def delete_topic(self, context: RequestContext, topic_arn: topicARN) -> None:
+        call_moto(context)
+        parsed_arn = parse_and_validate_topic_arn(topic_arn)
+        store = self.get_store(account_id=parsed_arn["account"], region_name=context.region)
+        topic_subscriptions = store.topic_subscriptions.pop(topic_arn, [])
+        for topic_sub in topic_subscriptions:
+            store.subscriptions.pop(topic_sub, None)
+
+        store.sns_tags.pop(topic_arn, None)
+
+    def create_topic(
+        self,
+        context: RequestContext,
+        name: topicName,
+        attributes: TopicAttributesMap = None,
+        tags: TagList = None,
+        data_protection_policy: attributeValue = None,
+    ) -> CreateTopicResponse:
+        moto_response = call_moto(context)
+        store = self.get_store(account_id=context.account_id, region_name=context.region)
+        topic_arn = moto_response["TopicArn"]
+        tag_resource_success = extract_tags(topic_arn, tags, True, store)
+        if not tag_resource_success:
+            raise InvalidParameterException(
+                "Invalid parameter: Tags Reason: Topic already exists with different tags"
+            )
+        if tags:
+            self.tag_resource(context=context, resource_arn=topic_arn, tags=tags)
+        store.topic_subscriptions.setdefault(topic_arn, [])
+        return CreateTopicResponse(TopicArn=topic_arn)
+
+
+def is_raw_message_delivery(susbcriber):
+    return susbcriber.get("RawMessageDelivery") in ("true", True, "True")
+
+
+def validate_subscription_attribute(
+    attribute_name: str, attribute_value: str, topic_arn: str
+) -> None:
+    """
+    Validate the subscription attribute to be set. See:
+    https://docs.aws.amazon.com/sns/latest/api/API_SetSubscriptionAttributes.html
+    :param attribute_name: the subscription attribute name, must be in VALID_SUBSCRIPTION_ATTR_NAME
+    :param attribute_value: the subscription attribute value
+    :param topic_arn: the topic_arn of the subscription, needed to know if it is FIFO
+    :raises InvalidParameterException
+    :return:
+    """
+    if attribute_name not in sns_constants.VALID_SUBSCRIPTION_ATTR_NAME:
+        raise InvalidParameterException("Invalid parameter: AttributeName")
+
+    if attribute_name == "FilterPolicy":
+        try:
+            json.loads(attribute_value or "{}")
+        except json.JSONDecodeError:
+            raise InvalidParameterException(
+                "Invalid parameter: FilterPolicy: failed to parse JSON."
+            )
+    elif attribute_name == "FilterPolicyScope":
+        if attribute_value not in ("MessageAttributes", "MessageBody"):
+            raise InvalidParameterException(
+                f"Invalid parameter: FilterPolicyScope: Invalid value [{attribute_value}]. Please use either MessageBody or MessageAttributes"
+            )
+    elif attribute_name == "RawMessageDelivery":
+        # TODO: only for SQS and https(s) subs, + firehose
+        return
+
+    elif attribute_name == "RedrivePolicy":
+        try:
+            dlq_target_arn = json.loads(attribute_value).get("deadLetterTargetArn", "")
+        except json.JSONDecodeError:
+            raise InvalidParameterException(
+                "Invalid parameter: RedrivePolicy: failed to parse JSON."
+            )
+        try:
+            parsed_arn = parse_arn(dlq_target_arn)
+        except InvalidArnException:
+            raise InvalidParameterException(
+                "Invalid parameter: RedrivePolicy: deadLetterTargetArn is an invalid arn"
+            )
 
-        object_attrs = request.get("ObjectAttributes", [])
-        response = GetObjectAttributesOutput()
-        if "ETag" in object_attrs:
-            response["ETag"] = s3_object.etag
-        if "StorageClass" in object_attrs:
-            response["StorageClass"] = s3_object.storage_class
-        if "ObjectSize" in object_attrs:
-            response["ObjectSize"] = s3_object.size
-        if "Checksum" in object_attrs and (checksum_algorithm := s3_object.checksum_algorithm):
-            response["Checksum"] = {  # noqa
-                f"Checksum{checksum_algorithm.upper()}": s3_object.checksum_value
-            }
+        if topic_arn.endswith(".fifo"):
+            if not parsed_arn["resource"].endswith(".fifo") or "sqs" not in parsed_arn["service"]:
+                raise InvalidParameterException(
+                    "Invalid parameter: RedrivePolicy: must use a FIFO queue as DLQ for a FIFO topic"
+                )
 
-        response["LastModified"] = s3_object.last_modified
 
-        if s3_bucket.versioning_status:
-            response["VersionId"] = s3_object.version_id
+def validate_message_attributes(message_attributes: MessageAttributeMap) -> None:
+    """
+    Validate the message attributes, and raises an exception if those do not follow AWS validation
+    See: https://docs.aws.amazon.com/sns/latest/dg/sns-message-attributes.html
+    Regex from: https://stackoverflow.com/questions/40718851/regex-that-does-not-allow-consecutive-dots
+    :param message_attributes: the message attributes map for the message
+    :raises: InvalidParameterValueException
+    :return: None
+    """
+    for attr_name, attr in message_attributes.items():
+        if len(attr_name) > 256:
+            raise InvalidParameterValueException(
+                "Length of message attribute name must be less than 256 bytes."
+            )
+        validate_message_attribute_name(attr_name)
+        # `DataType` is a required field for MessageAttributeValue
+        data_type = attr["DataType"]
+        if data_type not in (
+            "String",
+            "Number",
+            "Binary",
+        ) and not sns_constants.ATTR_TYPE_REGEX.match(data_type):
+            raise InvalidParameterValueException(
+                f"The message attribute '{attr_name}' has an invalid message attribute type, the set of supported type prefixes is Binary, Number, and String."
+            )
+        value_key_data_type = "Binary" if data_type.startswith("Binary") else "String"
+        value_key = f"{value_key_data_type}Value"
+        if value_key not in attr:
+            raise InvalidParameterValueException(
+                f"The message attribute '{attr_name}' with type '{data_type}' must use field '{value_key_data_type}'."
+            )
+        elif not attr[value_key]:
+            raise InvalidParameterValueException(
+                f"The message attribute '{attr_name}' must contain non-empty message attribute value for message attribute type '{data_type}'.",
+            )
 
-        # TODO implement PartNumber test once multipart is done
-        if s3_object.parts:
-            response["ObjectParts"] = GetObjectAttributesParts(TotalPartsCount=len(s3_object.parts))
 
-        return response
+def validate_message_attribute_name(name: str) -> None:
+    """
+    Validate the message attribute name with the specification of AWS.
+    The message attribute name can contain the following characters: A-Z, a-z, 0-9, underscore(_), hyphen(-), and period (.). The name must not start or end with a period, and it should not have successive periods.
+    :param name: message attribute name
+    :raises InvalidParameterValueException: if the name does not conform to the spec
+    """
+    if not sns_constants.MSG_ATTR_NAME_REGEX.match(name):
+        # find the proper exception
+        if name[0] == ".":
+            raise InvalidParameterValueException(
+                "Invalid message attribute name starting with character '.' was found."
+            )
+        elif name[-1] == ".":
+            raise InvalidParameterValueException(
+                "Invalid message attribute name ending with character '.' was found."
+            )
 
-    def restore_object(
-        self,
-        context: RequestContext,
-        bucket: BucketName,
-        key: ObjectKey,
-        version_id: ObjectVersionId = None,
-        restore_request: RestoreRequest = None,
-        request_payer: RequestPayer = None,
-        checksum_algorithm: ChecksumAlgorithm = None,
-        expected_bucket_owner: AccountId = None,
-    ) -> RestoreObjectOutput:
-        store = self.get_store(context.account_id, context.region)
-        if not (s3_bucket := store.buckets.get(bucket)):
-            raise NoSuchBucket("The specified bucket does not exist", BucketName=bucket)
+        for idx, char in enumerate(name):
+            if char not in sns_constants.VALID_MSG_ATTR_NAME_CHARS:
+                # change prefix from 0x to #x, without capitalizing the x
+                hex_char = "#x" + hex(ord(char)).upper()[2:]
+                raise InvalidParameterValueException(
+                    f"Invalid non-alphanumeric character '{hex_char}' was found in the message attribute name. Can only include alphanumeric characters, hyphens, underscores, or dots."
+                )
+            # even if we go negative index, it will be covered by starting/ending with dot
+            if char == "." and name[idx - 1] == ".":
+                raise InvalidParameterValueException(
+                    "Message attribute name can not have successive '.' character."
+                )
 
-        s3_object = s3_bucket.get_object(
-            key=key,
-            version_id=version_id,
-            http_method="GET",  # TODO: verify http method
-        )
-        if s3_object.storage_class not in ARCHIVES_STORAGE_CLASSES:
-            raise InvalidObjectState(StorageClass=s3_object.storage_class)
 
-        # TODO: moto was only supported "Days" parameters from RestoreRequest, and was ignoring the others
-        # will only implement only the same functionality for now
+def extract_tags(
+    topic_arn: str, tags: TagList, is_create_topic_request: bool, store: SnsStore
+) -> bool:
+    existing_tags = list(store.sns_tags.get(topic_arn, []))
+    # if this is none there is nothing to check
+    if topic_arn in store.topic_subscriptions:
+        if tags is None:
+            tags = []
+        for tag in tags:
+            # this means topic already created with empty tags and when we try to create it
+            # again with other tag value then it should fail according to aws documentation.
+            if is_create_topic_request and existing_tags is not None and tag not in existing_tags:
+                return False
+    return True
+
+
+def parse_and_validate_topic_arn(topic_arn: str) -> ArnData:
+    try:
+        return parse_arn(topic_arn)
+    except InvalidArnException:
+        count = len(topic_arn.split(":"))
+        raise InvalidParameterException(
+            f"Invalid parameter: TopicArn Reason: An ARN must have at least 6 elements, not {count}"
+        )
+
+
+def encode_subscription_token_with_region(region: str) -> str:
+    """
+    Create a 64 characters Subscription Token with the region encoded
+    :param region:
+    :return: a subscription token with the region encoded
+    """
+    return ((region.encode() + b"/").hex() + short_uid() * 8)[:64]
+
+
+def get_region_from_subscription_token(token: str) -> str:
+    """
+    Try to decode and return the region from a subscription token
+    :param token:
+    :return: the region if able to decode it
+    :raises: InvalidParameterException if the token is invalid
+    """
+    try:
+        region = token.split("2f", maxsplit=1)[0]
+        return bytes.fromhex(region).decode("utf-8")
+    except (IndexError, ValueError, TypeError, UnicodeDecodeError):
+        raise InvalidParameterException("Invalid parameter: Token")
+
+
+def register_sns_api_resource(router: Router):
+    """Register the retrospection endpoints as internal LocalStack endpoints."""
+    router.add(SNSServicePlatformEndpointMessagesApiResource())
+    router.add(SNSServiceSMSMessagesApiResource())
+
+
+def _format_messages(sent_messages: List[Dict[str, str]], validated_keys: List[str]):
+    """
+    This method format the messages to be more readable and undo the format change that was needed for Moto
+    Should be removed once we refactor SNS.
+    """
+    formatted_messages = []
+    for sent_message in sent_messages:
+        msg = {
+            key: json.dumps(value)
+            if key == "Message" and sent_message.get("MessageStructure") == "json"
+            else value
+            for key, value in sent_message.items()
+            if key in validated_keys
+        }
+        formatted_messages.append(msg)
+
+    return formatted_messages
+
+
+class SNSServicePlatformEndpointMessagesApiResource:
+    """Provides a REST API for retrospective access to platform endpoint messages sent via SNS.
+
+    This is registered as a LocalStack internal HTTP resource.
+
+    This endpoint accepts:
+    - GET param `accountId`: selector for AWS account. If not specified, return fallback `000000000000` test ID
+    - GET param `region`: selector for AWS `region`. If not specified, return default "us-east-1"
+    - GET param `endpointArn`: filter for `endpointArn` resource in SNS
+    - DELETE param `accountId`: selector for AWS account
+    - DELETE param `region`: will delete saved messages for `region`
+    - DELETE param `endpointArn`: will delete saved messages for `endpointArn`
+    """
+
+    _PAYLOAD_FIELDS = [
+        "TargetArn",
+        "TopicArn",
+        "Message",
+        "MessageAttributes",
+        "MessageStructure",
+        "Subject",
+        "MessageId",
+    ]
+
+    @route(sns_constants.PLATFORM_ENDPOINT_MSGS_ENDPOINT, methods=["GET"])
+    def on_get(self, request: Request):
+        account_id = request.args.get("accountId", get_aws_account_id())
+        region = request.args.get("region", "us-east-1")
+        filter_endpoint_arn = request.args.get("endpointArn")
+        store: SnsStore = sns_stores[account_id][region]
+        if filter_endpoint_arn:
+            messages = store.platform_endpoint_messages.get(filter_endpoint_arn, [])
+            messages = _format_messages(messages, self._PAYLOAD_FIELDS)
+            return {
+                "platform_endpoint_messages": {filter_endpoint_arn: messages},
+                "region": region,
+            }
 
-        # if a request was already done and the object was available, and we're updating it, set the status code to 200
-        status_code = 200 if s3_object.restore else 202
-        restore_days = restore_request.get("Days")
-        if not restore_days:
-            LOG.debug("LocalStack does not support restore SELECT requests yet.")
-            return RestoreObjectOutput()
+        platform_endpoint_messages = {
+            endpoint_arn: _format_messages(messages, self._PAYLOAD_FIELDS)
+            for endpoint_arn, messages in store.platform_endpoint_messages.items()
+        }
+        return {
+            "platform_endpoint_messages": platform_endpoint_messages,
+            "region": region,
+        }
+
+    @route(sns_constants.PLATFORM_ENDPOINT_MSGS_ENDPOINT, methods=["DELETE"])
+    def on_delete(self, request: Request) -> Response:
+        account_id = request.args.get("accountId", get_aws_account_id())
+        region = request.args.get("region", "us-east-1")
+        filter_endpoint_arn = request.args.get("endpointArn")
+        store: SnsStore = sns_stores[account_id][region]
+        if filter_endpoint_arn:
+            store.platform_endpoint_messages.pop(filter_endpoint_arn, None)
+            return Response("", status=204)
+
+        store.platform_endpoint_messages.clear()
+        return Response("", status=204)
+
+
+class SNSServiceSMSMessagesApiResource:
+    """Provides a REST API for retrospective access to SMS messages sent via SNS.
+
+    This is registered as a LocalStack internal HTTP resource.
+
+    This endpoint accepts:
+    - GET param `accountId`: selector for AWS account. If not specified, return fallback `000000000000` test ID
+    - GET param `region`: selector for AWS `region`. If not specified, return default "us-east-1"
+    - GET param `phoneNumber`: filter for `phoneNumber` resource in SNS
+    """
+
+    _PAYLOAD_FIELDS = [
+        "PhoneNumber",
+        "TopicArn",
+        "SubscriptionArn",
+        "MessageId",
+        "Message",
+        "MessageAttributes",
+        "MessageStructure",
+        "Subject",
+    ]
+
+    @route(sns_constants.SMS_MSGS_ENDPOINT, methods=["GET"])
+    def on_get(self, request: Request):
+        account_id = request.args.get("accountId", get_aws_account_id())
+        region = request.args.get("region", "us-east-1")
+        filter_phone_number = request.args.get("phoneNumber")
+        store: SnsStore = sns_stores[account_id][region]
+        if filter_phone_number:
+            messages = [
+                m for m in store.sms_messages if m.get("PhoneNumber") == filter_phone_number
+            ]
+            messages = _format_messages(messages, self._PAYLOAD_FIELDS)
+            return {
+                "sms_messages": {filter_phone_number: messages},
+                "region": region,
+            }
 
-        restore_expiration_date = add_expiration_days_to_datetime(
-            datetime.datetime.utcnow(), restore_days
-        )
-        # TODO: add a way to transition from ongoing-request=true to false? for now it is instant
-        s3_object.restore = f'ongoing-request="false", expiry-date="{restore_expiration_date}"'
+        sms_messages = {}
 
-        # TODO: request charged
-        return RestoreObjectOutput(StatusCode=status_code)
+        for m in _format_messages(store.sms_messages, self._PAYLOAD_FIELDS):
+            sms_messages.setdefault(m.get("PhoneNumber"), []).append(m)
 
+        return {
+            "sms_messages": sms_messages,
+            "region": region,
+        }
+
+    @route(sns_constants.SMS_MSGS_ENDPOINT, methods=["DELETE"])
+    def on_delete(self, request: Request) -> Response:
+        account_id = request.args.get("accountId", get_aws_account_id())
+        region = request.args.get("region", "us-east-1")
+        filter_phone_number = request.args.get("phoneNumber")
+        store: SnsStore = sns_stores[account_id][region]
+        if filter_phone_number:
+            store.sms_messages = [
+                m for m in store.sms_messages if m.get("PhoneNumber") != filter_phone_number
+            ]
+            return Response("", status=204)
 
-def generate_version_id(bucket_versioning_status: str) -> str | None:
-    if not bucket_versioning_status:
-        return None
-    # TODO: check VersionID format, could it be base64 urlsafe encoded?
-    return token_urlsafe(16) if bucket_versioning_status.lower() == "enabled" else "null"
-
-
-def add_encryption_to_response(response: dict, s3_object: S3Object):
-    if encryption := s3_object.encryption:
-        response["ServerSideEncryption"] = encryption
-        if encryption == ServerSideEncryption.aws_kms:
-            response["SSEKMSKeyId"] = s3_object.kms_key_id
-            if s3_object.bucket_key_enabled is not None:
-                response["BucketKeyEnabled"] = s3_object.bucket_key_enabled
+        store.sms_messages.clear()
+        return Response("", status=204)
```

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/storage/core.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/storage/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/v3/storage/ephemeral.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/v3/storage/ephemeral.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/virtual_host.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/s3/website_hosting.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/secretsmanager/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/ses/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sns/constants.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sns/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sns/publisher.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/constants.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/exceptions.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/query_api.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sqs/utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack-core-2.2.1.dev20230808152722/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component_base.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/program_state.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/program_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/packages.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/stores.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/sts/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/services/transcribe/provider.py` & `localstack-core-2.2.1.dev20230808152722/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/state/core.py` & `localstack-core-2.2.1.dev20230808152722/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/state/inspect.py` & `localstack-core-2.2.1.dev20230808152722/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/state/pickle.py` & `localstack-core-2.2.1.dev20230808152722/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/state/snapshot.py` & `localstack-core-2.2.1.dev20230808152722/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/asf_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/aws/util.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/filters.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/fixtures.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/marking.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/marking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/snapshot.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/pytest/util.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/scenario/provisioning.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/scenario/provisioning.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/prototype.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/report.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/transformer.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.2.1.dev20230808152722/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/cli.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/client.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/events.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/logger.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/metadata.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/publisher.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/analytics/usage.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/archives.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/asyncio.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/auth.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/arns.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/aws_models.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/aws_responses.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/aws_stack.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/client.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/client_types.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/queries.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/request_context.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/resources.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/aws/templating.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/bootstrap.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/collections.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/common.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/config_listener.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/container_networking.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/container_utils/container_client.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/coverage_docs.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/crypto.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/diagnose.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/docker_utils.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/files.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/functions.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/http.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/json.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/net.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/numbers.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/objects.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/patch.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/platform.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/run.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/scheduler.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/server/http2_server.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/server/proxy_server.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/serving.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/ssl.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/strings.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/sync.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/tagging.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/tail.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/testutil.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/threads.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/time.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/urls.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/venv.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack/utils/xml.py` & `localstack-core-2.2.1.dev20230808152722/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.2.1.dev20230808143011
+Version: 2.2.1.dev20230808152722
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/plux.json` & `localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/plux.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8796296296296295%*

 * *Differences: {"'localstack.hooks.on_infra_shutdown'": '{insert: [(1, '*

 * *                                         "'run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers')], "*

 * *                                         'delete: [0]}',*

 * * "'localstack.hooks.on_infra_start'": '{insert: [(2, '*

 * *                                      "'_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start'), "*

 * *                                      '(3, '*

 * *                                      "'_patch_botoco […]*

```diff
@@ -57,40 +57,40 @@
         "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file"
     ],
     "localstack.hooks.on_infra_ready": [
         "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
         "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
+        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
-        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
-        "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "deprecation_warnings=localstack.plugins:deprecation_warnings",
+        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
         "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
-        "deprecation_warnings=localstack.plugins:deprecation_warnings",
-        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener"
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
+        "_publish_container_info=localstack.runtime.analytics:_publish_container_info"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
-        "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
-        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
         "terraform/community=localstack.packages.plugins:terraform_package",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
         "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
         "local-kms/community=localstack.services.kms.plugins:local_kms_package",
         "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package"
+        "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
+        "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
+        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs"
     ]
 }
```

### Comparing `localstack-core-2.2.1.dev20230808143011/localstack_core.egg-info/requires.txt` & `localstack-core-2.2.1.dev20230808152722/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/pyproject.toml` & `localstack-core-2.2.1.dev20230808152722/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.2.1.dev20230808143011/setup.cfg` & `localstack-core-2.2.1.dev20230808152722/setup.cfg`

 * *Files identical despite different names*

