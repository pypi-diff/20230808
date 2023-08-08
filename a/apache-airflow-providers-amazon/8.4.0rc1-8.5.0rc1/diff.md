# Comparing `tmp/apache-airflow-providers-amazon-8.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-amazon-8.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-amazon-8.4.0rc1.tar", last modified: Sat Jul 29 12:07:48 2023, max compression
+gzip compressed data, was "apache-airflow-providers-amazon-8.5.0rc1.tar", last modified: Fri Aug  4 21:40:33 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.4.0rc1.tar` & `apache-airflow-providers-amazon-8.5.0rc1.tar`

### file list

```diff
@@ -1,199 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.319975 apache-airflow-providers-amazon-8.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-07-29 12:07:45.000000 apache-airflow-providers-amazon-8.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8040 2023-07-29 12:07:48.320623 apache-airflow-providers-amazon-8.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6055 2023-07-29 12:07:45.000000 apache-airflow-providers-amazon-8.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.708955 apache-airflow-providers-amazon-8.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.710281 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.769495 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-07-29 12:01:19.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.776381 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.916933 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12358 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    47454 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    21319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)    10541 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     4263 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/chime.py
--rw-r--r--   0 root         (0) root         (0)     3378 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14079 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7907 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23958 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12119 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    20679 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/eventbridge.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    16313 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7616 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     7931 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8095 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     5883 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15479 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8342 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    58255 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56469 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3463 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.936293 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.944820 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9600 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:47.950487 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/chime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.029836 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)    20436 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    33315 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    50133 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    74988 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/eventbridge.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     9663 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     7749 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    38326 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    32304 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    30235 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    61246 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     6411 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.038514 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.106360 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     9160 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     3721 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    22909 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3027 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    15066 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    12794 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9543 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.171760 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7019 2023-07-04 06:09:02.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6368 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8544 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8550 2023-07-16 17:25:26.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8865 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.217435 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2427 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/athena.py
--rw-r--r--   0 root         (0) root         (0)     5403 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/base.py
--rw-r--r--   0 root         (0) root         (0)    10713 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/batch.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/ec2.py
--rw-r--r--   0 root         (0) root         (0)     9049 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/ecs.py
--rw-r--r--   0 root         (0) root         (0)    16050 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/eks.py
--rw-r--r--   0 root         (0) root         (0)    19426 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/emr.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/glue.py
--rw-r--r--   0 root         (0) root         (0)     2622 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)    10046 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/rds.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/s3.py
--rw-r--r--   0 root         (0) root         (0)     7906 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2481 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.249327 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2968 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     4491 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/waiter.py
--rw-r--r--   0 root         (0) root         (0)     5890 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.293269 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/athena.json
--rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/batch.json
--rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json
--rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
--rw-r--r--   0 root         (0) root         (0)     4242 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/glue.json
--rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/redshift.json
--rw-r--r--   0 root         (0) root         (0)     5254 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
--rw-r--r--   0 root         (0) root         (0)     1034 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/stepfunctions.json
--rw-r--r--   0 root         (0) root         (0)    41325 2023-07-29 12:07:45.000000 apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:48.317181 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8040 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8718 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:07:47.000000 apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-amazon-8.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2252 2023-07-29 12:07:48.322543 apache-airflow-providers-amazon-8.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2502 2023-07-29 12:07:45.000000 apache-airflow-providers-amazon-8.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.772975 apache-airflow-providers-amazon-8.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-08-04 21:40:29.000000 apache-airflow-providers-amazon-8.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-amazon-8.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8204 2023-08-04 21:40:33.773963 apache-airflow-providers-amazon-8.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6191 2023-08-04 21:40:29.000000 apache-airflow-providers-amazon-8.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.071339 apache-airflow-providers-amazon-8.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.072927 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.155929 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-08-04 21:33:34.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.166339 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.363768 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12358 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    47454 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    21319 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)    10541 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/chime.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14079 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7907 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7928 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23958 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12119 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    20679 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-08-04 10:24:22.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/eventbridge.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    16313 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7616 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     7931 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15479 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13169 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8342 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     7160 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    58277 2023-08-04 10:24:22.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56469 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.383860 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.396192 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9600 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.403752 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/notifications/chime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.490115 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19662 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    20423 2023-08-04 10:24:22.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18421 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10720 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    33315 2023-08-04 21:09:30.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    50133 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    74988 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2023-08-04 10:24:22.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/eventbridge.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     9663 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2023-07-03 06:46:02.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    38629 2023-08-04 10:24:22.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    32304 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    30235 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    66643 2023-08-04 19:44:14.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     6411 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.500673 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.564986 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     9160 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3984 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-07-05 07:19:39.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    22909 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3719 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    15066 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    12794 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9793 2023-08-04 10:24:22.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.624786 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7019 2023-07-04 06:09:02.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     9841 2023-08-04 19:44:14.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4173 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5981 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8550 2023-07-16 17:25:26.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3643 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8865 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.669489 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/athena.py
+-rw-r--r--   0 root         (0) root         (0)     5403 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/base.py
+-rw-r--r--   0 root         (0) root         (0)    10713 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-29 05:49:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     9049 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    16050 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/eks.py
+-rw-r--r--   0 root         (0) root         (0)    19426 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/emr.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/glue.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)    10046 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/rds.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-07-09 14:40:47.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     9085 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/s3.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     7739 2023-08-04 10:24:22.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.705960 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2968 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20649 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 05:42:54.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     3271 2023-08-04 10:24:22.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     4491 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-06-29 05:49:30.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     5890 2023-06-30 08:49:17.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.747703 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-24 10:23:43.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/athena.json
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/batch.json
+-rw-r--r--   0 root         (0) root         (0)      895 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-17 16:45:00.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      851 2023-06-20 06:40:52.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-06-24 10:23:12.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-06-28 06:26:40.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-01 07:44:14.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/glue.json
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-01 06:14:28.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/redshift.json
+-rw-r--r--   0 root         (0) root         (0)     5254 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-26 06:59:50.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/stepfunctions.json
+-rw-r--r--   0 root         (0) root         (0)    41529 2023-08-04 21:40:29.000000 apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:33.770351 apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8204 2023-08-04 21:40:32.000000 apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8805 2023-08-04 21:40:32.000000 apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:32.000000 apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-08-04 21:40:32.000000 apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:32.000000 apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-08-04 21:40:32.000000 apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:32.000000 apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-amazon-8.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-08-04 21:40:33.776005 apache-airflow-providers-amazon-8.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-08-04 21:40:29.000000 apache-airflow-providers-amazon-8.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/LICENSE` & `apache-airflow-providers-amazon-8.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/MANIFEST.in` & `apache-airflow-providers-amazon-8.5.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/PKG-INFO` & `apache-airflow-providers-amazon-8.5.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.4.0rc1
+Version: 8.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -35,14 +35,15 @@
 Provides-Extra: exasol
 Provides-Extra: ftp
 Provides-Extra: google
 Provides-Extra: http
 Provides-Extra: imap
 Provides-Extra: microsoft.azure
 Provides-Extra: mongo
+Provides-Extra: openlineage
 Provides-Extra: salesforce
 Provides-Extra: ssh
 Provides-Extra: pandas
 Provides-Extra: aiobotocore
 License-File: LICENSE
 License-File: NOTICE
 
@@ -80,28 +81,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.4.0rc1``
+Release: ``8.5.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -153,13 +154,14 @@
 `apache-airflow-providers-exasol <https://airflow.apache.org/docs/apache-airflow-providers-exasol>`_                    ``exasol``
 `apache-airflow-providers-ftp <https://airflow.apache.org/docs/apache-airflow-providers-ftp>`_                          ``ftp``
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_                    ``google``
 `apache-airflow-providers-http <https://airflow.apache.org/docs/apache-airflow-providers-http>`_                        ``http``
 `apache-airflow-providers-imap <https://airflow.apache.org/docs/apache-airflow-providers-imap>`_                        ``imap``
 `apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
 `apache-airflow-providers-mongo <https://airflow.apache.org/docs/apache-airflow-providers-mongo>`_                      ``mongo``
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_          ``openlineage``
 `apache-airflow-providers-salesforce <https://airflow.apache.org/docs/apache-airflow-providers-salesforce>`_            ``salesforce``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                          ``ssh``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/README.rst` & `apache-airflow-providers-amazon-8.5.0rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.4.0rc1``
+Release: ``8.5.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -105,13 +105,14 @@
 `apache-airflow-providers-exasol <https://airflow.apache.org/docs/apache-airflow-providers-exasol>`_                    ``exasol``
 `apache-airflow-providers-ftp <https://airflow.apache.org/docs/apache-airflow-providers-ftp>`_                          ``ftp``
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_                    ``google``
 `apache-airflow-providers-http <https://airflow.apache.org/docs/apache-airflow-providers-http>`_                        ``http``
 `apache-airflow-providers-imap <https://airflow.apache.org/docs/apache-airflow-providers-imap>`_                        ``imap``
 `apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
 `apache-airflow-providers-mongo <https://airflow.apache.org/docs/apache-airflow-providers-mongo>`_                      ``mongo``
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_          ``openlineage``
 `apache-airflow-providers-salesforce <https://airflow.apache.org/docs/apache-airflow-providers-salesforce>`_            ``salesforce``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                          ``ssh``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "8.4.0"
+__version__ = "8.5.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/chime.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/chime.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/eventbridge.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+
 from __future__ import annotations
 
-from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
+from enum import Enum
 
 
-class EventBridgeHook(AwsBaseHook):
-    """Amazon EventBridge Hook."""
+class ApprovalStatus(Enum):
+    """Approval statuses for a Sagemaker Model Package."""
 
-    def __init__(self, *args, **kwargs):
-        """Creating object."""
-        super().__init__(client_type="events", *args, **kwargs)
+    APPROVED = "Approved"
+    REJECTED = "Rejected"
+    PENDING_MANUAL_APPROVAL = "PendingManualApproval"
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.amazon.aws.exceptions import S3HookUriParseFailure
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.providers.amazon.aws.utils.tags import format_tags
 from airflow.utils.helpers import chunks
 
 if TYPE_CHECKING:
-    from mypy_boto3_s3.service_resource import Object as S3ResourceObject
+    from mypy_boto3_s3.service_resource import Bucket as S3Bucket, Object as S3ResourceObject
 
 T = TypeVar("T", bound=Callable)
 
 logger = logging.getLogger(__name__)
 
 
 def provide_bucket_name(func: T) -> T:
@@ -294,15 +294,15 @@
                 self.log.error(
                     'Access to bucket "%s" is forbidden or there was an error with the request', bucket_name
                 )
                 self.log.error(e)
             return False
 
     @provide_bucket_name
-    def get_bucket(self, bucket_name: str | None = None) -> object:
+    def get_bucket(self, bucket_name: str | None = None) -> S3Bucket:
         """
         Returns a :py:class:`S3.Bucket` object.
 
         .. seealso::
             - :external+boto3:py:meth:`S3.ServiceResource.Bucket`
 
         :param bucket_name: the name of the bucket
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/notifications/chime.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/notifications/chime.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         array_properties: dict | None = None,
         node_overrides: dict | None = None,
         share_identifier: str | None = None,
         scheduling_priority_override: int | None = None,
         parameters: dict | None = None,
         job_id: str | None = None,
         waiters: Any | None = None,
-        max_retries: int | None = None,
+        max_retries: int = 4200,
         status_retries: int | None = None,
         aws_conn_id: str | None = None,
         region_name: str | None = None,
         tags: dict | None = None,
         wait_for_completion: bool = True,
         deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         poll_interval: int = 30,
@@ -219,15 +219,15 @@
         self.submit_job(context)
 
         if self.deferrable:
             self.defer(
                 timeout=self.execution_timeout,
                 trigger=BatchJobTrigger(
                     job_id=self.job_id,
-                    waiter_max_attempts=self.max_retries or 10,
+                    waiter_max_attempts=self.max_retries,
                     aws_conn_id=self.aws_conn_id,
                     region_name=self.region_name,
                     waiter_delay=self.poll_interval,
                 ),
                 method_name="execute_complete",
             )
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/eventbridge.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -10,78 +11,60 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+"""This module contains base AWS to AWS transfer operator."""
 from __future__ import annotations
 
-from functools import cached_property
-from typing import TYPE_CHECKING, Sequence
+import warnings
+from typing import Sequence
 
-from airflow import AirflowException
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
-from airflow.providers.amazon.aws.hooks.eventbridge import EventBridgeHook
-from airflow.providers.amazon.aws.utils import trim_none_values
+from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
+from airflow.utils.types import NOTSET, ArgNotSet
 
-if TYPE_CHECKING:
-    from airflow.utils.context import Context
+_DEPRECATION_MSG = (
+    "The aws_conn_id parameter has been deprecated. Use the source_aws_conn_id parameter instead."
+)
 
 
-class EventBridgePutEventsOperator(BaseOperator):
+class AwsToAwsBaseOperator(BaseOperator):
     """
-    Put Events onto Amazon EventBridge.
+    Base class for AWS to AWS transfer operators.
 
-    :param entries: the list of events to be put onto EventBridge, each event is a dict (required)
-    :param endpoint_id: the URL subdomain of the endpoint
-    :param aws_conn_id: the AWS connection to use
-    :param region_name: the region where events are to be sent
+    :param source_aws_conn_id: The Airflow connection used for AWS credentials
+        to access DynamoDB. If this is None or empty then the default boto3
+        behaviour is used. If running Airflow in a distributed manner and
+        source_aws_conn_id is None or empty, then default boto3 configuration
+        would be used (and must be maintained on each worker node).
+    :param dest_aws_conn_id: The Airflow connection used for AWS credentials
+        to access S3. If this is not set then the source_aws_conn_id connection is used.
+    :param aws_conn_id: The Airflow connection used for AWS credentials (deprecated; use source_aws_conn_id).
 
     """
 
-    template_fields: Sequence[str] = ("entries", "endpoint_id", "aws_conn_id", "region_name")
+    template_fields: Sequence[str] = (
+        "source_aws_conn_id",
+        "dest_aws_conn_id",
+    )
 
     def __init__(
         self,
         *,
-        entries: list[dict],
-        endpoint_id: str | None = None,
-        aws_conn_id: str = "aws_default",
-        region_name: str | None = None,
+        source_aws_conn_id: str | None = AwsBaseHook.default_conn_name,
+        dest_aws_conn_id: str | None | ArgNotSet = NOTSET,
+        aws_conn_id: str | None | ArgNotSet = NOTSET,
         **kwargs,
-    ):
+    ) -> None:
         super().__init__(**kwargs)
-        self.entries = entries
-        self.endpoint_id = endpoint_id
-        self.aws_conn_id = aws_conn_id
-        self.region_name = region_name
-
-    @cached_property
-    def hook(self) -> EventBridgeHook:
-        """Create and return an EventBridgeHook."""
-        return EventBridgeHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
-
-    def execute(self, context: Context):
-
-        response = self.hook.conn.put_events(
-            **trim_none_values(
-                {
-                    "Entries": self.entries,
-                    "EndpointId": self.endpoint_id,
-                }
-            )
+        if not isinstance(aws_conn_id, ArgNotSet):
+            warnings.warn(_DEPRECATION_MSG, AirflowProviderDeprecationWarning, stacklevel=3)
+            self.source_aws_conn_id = aws_conn_id
+        else:
+            self.source_aws_conn_id = source_aws_conn_id
+        self.dest_aws_conn_id = (
+            self.source_aws_conn_id if isinstance(dest_aws_conn_id, ArgNotSet) else dest_aws_conn_id
         )
-
-        self.log.info("Sent %d events to EventBridge.", len(self.entries))
-
-        if response.get("FailedEntryCount"):
-            for event in response["Entries"]:
-                if "ErrorCode" in event:
-                    self.log.error(event)
-
-            raise AirflowException(
-                f"{response['FailedEntryCount']} entries in this request have failed to send."
-            )
-
-        if self.do_xcom_push:
-            return [e["EventId"] for e in response["Entries"]]
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/rds.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,42 +388,49 @@
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:RdsCancelExportTaskOperator`
 
     :param export_task_identifier: The identifier of the snapshot export task to cancel
     :param wait_for_completion:  If True, waits for DB snapshot export to cancel. (default: True)
+    :param check_interval: The amount of time in seconds to wait between attempts
+    :param max_attempts: The maximum number of attempts to be made
     """
 
     template_fields = ("export_task_identifier",)
 
     def __init__(
         self,
         *,
         export_task_identifier: str,
         wait_for_completion: bool = True,
         check_interval: int = 30,
+        max_attempts: int = 40,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.export_task_identifier = export_task_identifier
         self.wait_for_completion = wait_for_completion
         self.check_interval = check_interval
+        self.max_attempts = max_attempts
 
     def execute(self, context: Context) -> str:
         self.log.info("Canceling export task %s", self.export_task_identifier)
 
         cancel_export = self.hook.conn.cancel_export_task(
             ExportTaskIdentifier=self.export_task_identifier,
         )
 
         if self.wait_for_completion:
             self.hook.wait_for_export_task_state(
-                self.export_task_identifier, target_state="canceled", check_interval=self.check_interval
+                self.export_task_identifier,
+                target_state="canceled",
+                check_interval=self.check_interval,
+                max_attempts=self.max_attempts,
             )
         return json.dumps(cancel_export, default=str)
 
 
 class RdsCreateEventSubscriptionOperator(RdsBaseOperator):
     """
     Creates an RDS event notification subscription.
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,21 +36,24 @@
 )
 from airflow.providers.amazon.aws.utils import trim_none_values
 from airflow.providers.amazon.aws.utils.sagemaker import ApprovalStatus
 from airflow.providers.amazon.aws.utils.tags import format_tags
 from airflow.utils.json import AirflowJsonEncoder
 
 if TYPE_CHECKING:
+    from openlineage.client.run import Dataset
+
+    from airflow.providers.openlineage.extractors.base import OperatorLineage
     from airflow.utils.context import Context
 
 DEFAULT_CONN_ID: str = "aws_default"
 CHECK_INTERVAL_SECOND: int = 30
 
 
-def serialize(result: dict) -> str:
+def serialize(result: dict) -> dict:
     return json.loads(json.dumps(result, cls=AirflowJsonEncoder))
 
 
 class SageMakerBaseOperator(BaseOperator):
     """This is the base operator for all SageMaker operators.
 
     :param config: The configuration necessary to start a training job (templated)
@@ -154,14 +157,22 @@
         raise NotImplementedError("Please implement execute() in sub class!")
 
     @cached_property
     def hook(self):
         """Return SageMakerHook."""
         return SageMakerHook(aws_conn_id=self.aws_conn_id)
 
+    @staticmethod
+    def path_to_s3_dataset(path) -> Dataset:
+        from openlineage.client.run import Dataset
+
+        path = path.replace("s3://", "")
+        split_path = path.split("/")
+        return Dataset(namespace=f"s3://{split_path[0]}", name="/".join(split_path[1:]), facets={})
+
 
 class SageMakerProcessingOperator(SageMakerBaseOperator):
     """
     Use Amazon SageMaker Processing to analyze data and evaluate machine learning models on Amazon SageMaker.
 
     With Processing, you can use a simplified, managed experience on SageMaker
     to run your data processing workloads, such as feature engineering, data
@@ -221,14 +232,15 @@
         self.action_if_job_exists = action_if_job_exists
         self.wait_for_completion = wait_for_completion
         self.print_log = print_log
         self.check_interval = check_interval
         self.max_attempts = max_attempts or 60
         self.max_ingestion_time = max_ingestion_time
         self.deferrable = deferrable
+        self.serialized_job: dict
 
     def _create_integer_fields(self) -> None:
         """Set fields which should be cast to integers."""
         self.integer_fields: list[list[str] | list[list[str]]] = [
             ["ProcessingResources", "ClusterConfig", "InstanceCount"],
             ["ProcessingResources", "ClusterConfig", "VolumeSizeInGB"],
         ]
@@ -278,22 +290,56 @@
                     poke_interval=self.check_interval,
                     max_attempts=self.max_attempts,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
             )
 
-        return {"Processing": serialize(self.hook.describe_processing_job(self.config["ProcessingJobName"]))}
+        self.serialized_job = serialize(self.hook.describe_processing_job(self.config["ProcessingJobName"]))
+        return {"Processing": self.serialized_job}
 
     def execute_complete(self, context, event=None):
         if event["status"] != "success":
             raise AirflowException(f"Error while running job: {event}")
         else:
             self.log.info(event["message"])
-        return {"Processing": serialize(self.hook.describe_processing_job(self.config["ProcessingJobName"]))}
+        self.serialized_job = serialize(self.hook.describe_processing_job(self.config["ProcessingJobName"]))
+        return {"Processing": self.serialized_job}
+
+    def get_openlineage_facets_on_complete(self, task_instance) -> OperatorLineage:
+        """Returns OpenLineage data gathered from SageMaker's API response saved by processing job."""
+        from airflow.providers.openlineage.extractors.base import OperatorLineage
+
+        inputs = []
+        outputs = []
+        try:
+            inputs, outputs = self._extract_s3_dataset_identifiers(
+                processing_inputs=self.serialized_job["ProcessingInputs"],
+                processing_outputs=self.serialized_job["ProcessingOutputConfig"]["Outputs"],
+            )
+        except KeyError:
+            self.log.exception("Could not find input/output information in Xcom.")
+
+        return OperatorLineage(inputs=inputs, outputs=outputs)
+
+    def _extract_s3_dataset_identifiers(self, processing_inputs, processing_outputs):
+        inputs = []
+        outputs = []
+        try:
+            for processing_input in processing_inputs:
+                inputs.append(self.path_to_s3_dataset(processing_input["S3Input"]["S3Uri"]))
+        except KeyError:
+            self.log.exception("Cannot find S3 input details", exc_info=True)
+
+        try:
+            for processing_output in processing_outputs:
+                outputs.append(self.path_to_s3_dataset(processing_output["S3Output"]["S3Uri"]))
+        except KeyError:
+            self.log.exception("Cannot find S3 output details.", exc_info=True)
+        return inputs, outputs
 
 
 class SageMakerEndpointConfigOperator(SageMakerBaseOperator):
     """
     Creates an endpoint configuration that Amazon SageMaker hosting services uses to deploy models.
 
     In the configuration, you identify one or more models, created using the CreateModel API, to deploy and
@@ -575,14 +621,16 @@
             self.action_if_job_exists = action_if_job_exists
         else:
             raise AirflowException(
                 f"Argument action_if_job_exists accepts only 'timestamp', 'increment' and 'fail'. \
                 Provided value: '{action_if_job_exists}'."
             )
         self.deferrable = deferrable
+        self.serialized_model: dict
+        self.serialized_tranform: dict
 
     def _create_integer_fields(self) -> None:
         """Set fields which should be cast to integers."""
         self.integer_fields: list[list[str]] = [
             ["Transform", "TransformResources", "InstanceCount"],
             ["Transform", "MaxConcurrentTransforms"],
             ["Transform", "MaxPayloadInMB"],
@@ -646,29 +694,82 @@
                     poke_interval=self.check_interval,
                     max_attempts=self.max_attempts,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
             )
 
-        return {
-            "Model": serialize(self.hook.describe_model(transform_config["ModelName"])),
-            "Transform": serialize(self.hook.describe_transform_job(transform_config["TransformJobName"])),
-        }
+        self.serialized_model = serialize(self.hook.describe_model(transform_config["ModelName"]))
+        self.serialized_tranform = serialize(
+            self.hook.describe_transform_job(transform_config["TransformJobName"])
+        )
+        return {"Model": self.serialized_model, "Transform": self.serialized_tranform}
 
     def execute_complete(self, context, event=None):
         if event["status"] != "success":
             raise AirflowException(f"Error while running job: {event}")
         else:
             self.log.info(event["message"])
         transform_config = self.config.get("Transform", self.config)
-        return {
-            "Model": serialize(self.hook.describe_model(transform_config["ModelName"])),
-            "Transform": serialize(self.hook.describe_transform_job(transform_config["TransformJobName"])),
-        }
+        self.serialized_model = serialize(self.hook.describe_model(transform_config["ModelName"]))
+        self.serialized_tranform = serialize(
+            self.hook.describe_transform_job(transform_config["TransformJobName"])
+        )
+        return {"Model": self.serialized_model, "Transform": self.serialized_tranform}
+
+    def get_openlineage_facets_on_complete(self, task_instance) -> OperatorLineage:
+        """Returns OpenLineage data gathered from SageMaker's API response saved by transform job."""
+        from airflow.providers.openlineage.extractors import OperatorLineage
+
+        model_package_arn = None
+        transform_input = None
+        transform_output = None
+
+        try:
+            model_package_arn = self.serialized_model["PrimaryContainer"]["ModelPackageName"]
+        except KeyError:
+            self.log.error("Cannot find Model Package Name.", exc_info=True)
+
+        try:
+            transform_input = self.serialized_tranform["TransformInput"]["DataSource"]["S3DataSource"][
+                "S3Uri"
+            ]
+            transform_output = self.serialized_tranform["TransformOutput"]["S3OutputPath"]
+        except KeyError:
+            self.log.error("Cannot find some required input/output details.", exc_info=True)
+
+        inputs = []
+
+        if transform_input is not None:
+            inputs.append(self.path_to_s3_dataset(transform_input))
+
+        if model_package_arn is not None:
+            model_data_urls = self._get_model_data_urls(model_package_arn)
+            for model_data_url in model_data_urls:
+                inputs.append(self.path_to_s3_dataset(model_data_url))
+
+        outputs = []
+        if transform_output is not None:
+            outputs.append(self.path_to_s3_dataset(transform_output))
+
+        return OperatorLineage(inputs=inputs, outputs=outputs)
+
+    def _get_model_data_urls(self, model_package_arn) -> list:
+        model_data_urls = []
+        try:
+            model_containers = self.hook.get_conn().describe_model_package(
+                ModelPackageName=model_package_arn
+            )["InferenceSpecification"]["Containers"]
+
+            for container in model_containers:
+                model_data_urls.append(container["ModelDataUrl"])
+        except KeyError:
+            self.log.exception("Cannot retrieve model details.", exc_info=True)
+
+        return model_data_urls
 
 
 class SageMakerTuningOperator(SageMakerBaseOperator):
     """
     Starts a hyperparameter tuning job.
 
     A hyperparameter tuning job finds the best version of a model by running
@@ -887,14 +988,15 @@
             self.action_if_job_exists = action_if_job_exists
         else:
             raise AirflowException(
                 f"Argument action_if_job_exists accepts only 'timestamp', 'increment' and 'fail'. \
                 Provided value: '{action_if_job_exists}'."
             )
         self.deferrable = deferrable
+        self.serialized_training_data: dict
 
     def expand_role(self) -> None:
         """Expands an IAM role name into an ARN."""
         if "RoleArn" in self.config:
             hook = AwsBaseHook(self.aws_conn_id, client_type="iam")
             self.config["RoleArn"] = hook.expand_role(self.config["RoleArn"])
 
@@ -947,24 +1049,48 @@
                     poke_interval=self.check_interval,
                     max_attempts=self.max_attempts,
                     aws_conn_id=self.aws_conn_id,
                 ),
                 method_name="execute_complete",
             )
 
-        result = {"Training": serialize(self.hook.describe_training_job(self.config["TrainingJobName"]))}
-        return result
+        self.serialized_training_data = serialize(
+            self.hook.describe_training_job(self.config["TrainingJobName"])
+        )
+        return {"Training": self.serialized_training_data}
 
     def execute_complete(self, context, event=None):
         if event["status"] != "success":
             raise AirflowException(f"Error while running job: {event}")
         else:
             self.log.info(event["message"])
-        result = {"Training": serialize(self.hook.describe_training_job(self.config["TrainingJobName"]))}
-        return result
+        self.serialized_training_data = serialize(
+            self.hook.describe_training_job(self.config["TrainingJobName"])
+        )
+        return {"Training": self.serialized_training_data}
+
+    def get_openlineage_facets_on_complete(self, task_instance) -> OperatorLineage:
+        """Returns OpenLineage data gathered from SageMaker's API response saved by training job."""
+        from airflow.providers.openlineage.extractors import OperatorLineage
+
+        inputs = []
+        outputs = []
+        try:
+            for input_data in self.serialized_training_data["InputDataConfig"]:
+                inputs.append(self.path_to_s3_dataset(input_data["DataSource"]["S3DataSource"]["S3Uri"]))
+        except KeyError:
+            self.log.exception("Issues extracting inputs.")
+
+        try:
+            outputs.append(
+                self.path_to_s3_dataset(self.serialized_training_data["ModelArtifacts"]["S3ModelArtifacts"])
+            )
+        except KeyError:
+            self.log.exception("Issues extracting inputs.")
+        return OperatorLineage(inputs=inputs, outputs=outputs)
 
 
 class SageMakerDeleteModelOperator(SageMakerBaseOperator):
     """
     Deletes a SageMaker model.
 
     .. seealso::
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/sqs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -11,50 +10,32 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Reads and then deletes the message from SQS queue."""
 from __future__ import annotations
 
-import json
-from functools import cached_property
-from typing import TYPE_CHECKING, Any, Collection, Literal, Sequence
-
-from deprecated import deprecated
-from jsonpath_ng import parse
+import asyncio
+from typing import Any, AsyncIterator, Collection, Literal
 
 from airflow.exceptions import AirflowException
 from airflow.providers.amazon.aws.hooks.base_aws import BaseAwsConnection
 from airflow.providers.amazon.aws.hooks.sqs import SqsHook
-from airflow.sensors.base import BaseSensorOperator
+from airflow.providers.amazon.aws.utils.sqs import process_response
+from airflow.triggers.base import BaseTrigger, TriggerEvent
 
-if TYPE_CHECKING:
-    from airflow.utils.context import Context
 
-
-class SqsSensor(BaseSensorOperator):
+class SqsSensorTrigger(BaseTrigger):
     """
-    Get messages from an Amazon SQS queue and then delete the messages from the queue.
-
-    If deletion of messages fails, an AirflowException is thrown. Otherwise, the messages
-    are pushed through XCom with the key ``messages``.
-
-    By default,the sensor performs one and only one SQS call per poke, which limits the result to
-    a maximum of 10 messages. However, the total number of SQS API calls per poke can be controlled
-    by num_batches param.
-
-    .. seealso::
-        For more information on how to use this sensor, take a look at the guide:
-        :ref:`howto/sensor:SqsSensor`
+    Asynchronously get messages from an Amazon SQS queue and then delete the messages from the queue.
 
+    :param sqs_queue: The SQS queue url
     :param aws_conn_id: AWS connection id
-    :param sqs_queue: The SQS queue url (templated)
     :param max_messages: The maximum number of messages to retrieve for each poke (templated)
     :param num_batches: The number of times the sensor will call the SQS API to receive messages (default: 1)
     :param wait_time_seconds: The time in seconds to wait for receiving messages (default: 1 second)
     :param visibility_timeout: Visibility timeout, a period of time during which
         Amazon SQS prevents other consumers from receiving and processing the message.
     :param message_filtering: Specified how received messages should be filtered. Supported options are:
         `None` (no filtering, default), `'literal'` (message Body literal match) or `'jsonpath'`
@@ -66,162 +47,122 @@
         and may match any of the specified values.
     :param message_filtering_config: Additional configuration to pass to the message filter.
         For example with JSONPath filtering you can pass a JSONPath expression string here,
         such as `'foo[*].baz'`. Messages with a Body which does not match are ignored.
     :param delete_message_on_reception: Default to `True`, the messages are deleted from the queue
         as soon as being consumed. Otherwise, the messages remain in the queue after consumption and
         should be deleted manually.
-
+    :param waiter_delay: The time in seconds to wait between calls to the SQS API to receive messages.
     """
 
-    template_fields: Sequence[str] = ("sqs_queue", "max_messages", "message_filtering_config")
-
     def __init__(
         self,
-        *,
-        sqs_queue,
+        sqs_queue: str,
         aws_conn_id: str = "aws_default",
         max_messages: int = 5,
         num_batches: int = 1,
         wait_time_seconds: int = 1,
         visibility_timeout: int | None = None,
         message_filtering: Literal["literal", "jsonpath"] | None = None,
         message_filtering_match_values: Any = None,
         message_filtering_config: Any = None,
         delete_message_on_reception: bool = True,
-        **kwargs,
+        waiter_delay: int = 60,
     ):
-        super().__init__(**kwargs)
         self.sqs_queue = sqs_queue
         self.aws_conn_id = aws_conn_id
         self.max_messages = max_messages
         self.num_batches = num_batches
         self.wait_time_seconds = wait_time_seconds
         self.visibility_timeout = visibility_timeout
-
         self.message_filtering = message_filtering
-
         self.delete_message_on_reception = delete_message_on_reception
-
-        if message_filtering_match_values is not None:
-            if not isinstance(message_filtering_match_values, set):
-                message_filtering_match_values = set(message_filtering_match_values)
         self.message_filtering_match_values = message_filtering_match_values
+        self.message_filtering_config = message_filtering_config
+        self.waiter_delay = waiter_delay
 
-        if self.message_filtering == "literal":
-            if self.message_filtering_match_values is None:
-                raise TypeError("message_filtering_match_values must be specified for literal matching")
+    def serialize(self) -> tuple[str, dict[str, Any]]:
+        return (
+            self.__class__.__module__ + "." + self.__class__.__qualname__,
+            {
+                "sqs_queue": self.sqs_queue,
+                "aws_conn_id": self.aws_conn_id,
+                "max_messages": self.max_messages,
+                "num_batches": self.num_batches,
+                "wait_time_seconds": self.wait_time_seconds,
+                "visibility_timeout": self.visibility_timeout,
+                "message_filtering": self.message_filtering,
+                "delete_message_on_reception": self.delete_message_on_reception,
+                "message_filtering_match_values": self.message_filtering_match_values,
+                "message_filtering_config": self.message_filtering_config,
+                "waiter_delay": self.waiter_delay,
+            },
+        )
 
-        self.message_filtering_config = message_filtering_config
+    @property
+    def hook(self) -> SqsHook:
+        return SqsHook(aws_conn_id=self.aws_conn_id)
 
-    def poll_sqs(self, sqs_conn: BaseAwsConnection) -> Collection:
+    async def poll_sqs(self, client: BaseAwsConnection) -> Collection:
         """
-        Poll SQS queue to retrieve messages.
+        Asynchronously poll SQS queue to retrieve messages.
 
-        :param sqs_conn: SQS connection
+        :param client: SQS connection
         :return: A list of messages retrieved from SQS
         """
         self.log.info("SqsSensor checking for message on queue: %s", self.sqs_queue)
 
         receive_message_kwargs = {
             "QueueUrl": self.sqs_queue,
             "MaxNumberOfMessages": self.max_messages,
             "WaitTimeSeconds": self.wait_time_seconds,
         }
         if self.visibility_timeout is not None:
             receive_message_kwargs["VisibilityTimeout"] = self.visibility_timeout
 
-        response = sqs_conn.receive_message(**receive_message_kwargs)
+        response = await client.receive_message(**receive_message_kwargs)
+        return response
 
-        if "Messages" not in response:
-            return []
-
-        messages = response["Messages"]
-        num_messages = len(messages)
-        self.log.info("Received %d messages", num_messages)
-
-        if num_messages and self.message_filtering:
-            messages = self.filter_messages(messages)
-            num_messages = len(messages)
-            self.log.info("There are %d messages left after filtering", num_messages)
-        return messages
-
-    def poke(self, context: Context):
-        """
-        Check subscribed queue for messages and write them to xcom with the ``messages`` key.
-
-        :param context: the context object
-        :return: ``True`` if message is available or ``False``
-        """
+    async def poke(self, client: Any):
         message_batch: list[Any] = []
-
-        # perform multiple SQS call to retrieve messages in series
         for _ in range(self.num_batches):
-            messages = self.poll_sqs(sqs_conn=self.hook.conn)
+            self.log.info("starting call to poll sqs")
+            response = await self.poll_sqs(client=client)
+            messages = process_response(
+                response,
+                self.message_filtering,
+                self.message_filtering_match_values,
+                self.message_filtering_config,
+            )
 
-            if not len(messages):
+            if not messages:
                 continue
 
             message_batch.extend(messages)
 
             if self.delete_message_on_reception:
-
                 self.log.info("Deleting %d messages", len(messages))
 
                 entries = [
                     {"Id": message["MessageId"], "ReceiptHandle": message["ReceiptHandle"]}
                     for message in messages
                 ]
-                response = self.hook.conn.delete_message_batch(QueueUrl=self.sqs_queue, Entries=entries)
+                response = await client.delete_message_batch(QueueUrl=self.sqs_queue, Entries=entries)
 
                 if "Successful" not in response:
                     raise AirflowException(
-                        "Delete SQS Messages failed " + str(response) + " for messages " + str(messages)
+                        f"Delete SQS Messages failed {str(response)} for messages {str(messages)}"
                     )
-        if not len(message_batch):
-            return False
 
-        context["ti"].xcom_push(key="messages", value=message_batch)
-        return True
+        return message_batch
 
-    @deprecated(reason="use `hook` property instead.")
-    def get_hook(self) -> SqsHook:
-        """Create and return an SqsHook."""
-        return self.hook
-
-    @cached_property
-    def hook(self) -> SqsHook:
-        return SqsHook(aws_conn_id=self.aws_conn_id)
-
-    def filter_messages(self, messages):
-        if self.message_filtering == "literal":
-            return self.filter_messages_literal(messages)
-        if self.message_filtering == "jsonpath":
-            return self.filter_messages_jsonpath(messages)
-        else:
-            raise NotImplementedError("Override this method to define custom filters")
-
-    def filter_messages_literal(self, messages):
-        filtered_messages = []
-        for message in messages:
-            if message["Body"] in self.message_filtering_match_values:
-                filtered_messages.append(message)
-        return filtered_messages
-
-    def filter_messages_jsonpath(self, messages):
-        jsonpath_expr = parse(self.message_filtering_config)
-        filtered_messages = []
-        for message in messages:
-            body = message["Body"]
-            # Body is a string, deserialize to an object and then parse
-            body = json.loads(body)
-            results = jsonpath_expr.find(body)
-            if not results:
-                continue
-            if self.message_filtering_match_values is None:
-                filtered_messages.append(message)
-                continue
-            for result in results:
-                if result.value in self.message_filtering_match_values:
-                    filtered_messages.append(message)
+    async def run(self) -> AsyncIterator[TriggerEvent]:
+        while True:
+            # This loop will run indefinitely until the timeout, which is set in the self.defer
+            # method, is reached.
+            async with self.hook.async_conn as client:
+                result = await self.poke(client=client)
+                if result:
+                    yield TriggerEvent({"status": "success", "message_batch": result})
                     break
-        return filtered_messages
+                else:
+                    await asyncio.sleep(self.waiter_delay)
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/azure_blob_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -11,60 +10,56 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""This module contains base AWS to AWS transfer operator."""
 from __future__ import annotations
 
 import warnings
-from typing import Sequence
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
-from airflow.models import BaseOperator
-from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
-from airflow.utils.types import NOTSET, ArgNotSet
-
-_DEPRECATION_MSG = (
-    "The aws_conn_id parameter has been deprecated. Use the source_aws_conn_id parameter instead."
-)
+from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
+from airflow.providers.amazon.aws.hooks.glue_crawler import GlueCrawlerHook
+from airflow.providers.amazon.aws.triggers.base import AwsBaseWaiterTrigger
 
 
-class AwsToAwsBaseOperator(BaseOperator):
+class GlueCrawlerCompleteTrigger(AwsBaseWaiterTrigger):
     """
-    Base class for AWS to AWS transfer operators.
-
-    :param source_aws_conn_id: The Airflow connection used for AWS credentials
-        to access DynamoDB. If this is None or empty then the default boto3
-        behaviour is used. If running Airflow in a distributed manner and
-        source_aws_conn_id is None or empty, then default boto3 configuration
-        would be used (and must be maintained on each worker node).
-    :param dest_aws_conn_id: The Airflow connection used for AWS credentials
-        to access S3. If this is not set then the source_aws_conn_id connection is used.
-    :param aws_conn_id: The Airflow connection used for AWS credentials (deprecated; use source_aws_conn_id).
+    Watches for a glue crawl, triggers when it finishes.
 
+    :param crawler_name: name of the crawler to watch
+    :param poll_interval: The amount of time in seconds to wait between attempts.
+    :param aws_conn_id: The Airflow connection used for AWS credentials.
     """
 
-    template_fields: Sequence[str] = (
-        "source_aws_conn_id",
-        "dest_aws_conn_id",
-    )
-
     def __init__(
         self,
-        *,
-        source_aws_conn_id: str | None = AwsBaseHook.default_conn_name,
-        dest_aws_conn_id: str | None | ArgNotSet = NOTSET,
-        aws_conn_id: str | None | ArgNotSet = NOTSET,
-        **kwargs,
-    ) -> None:
-        super().__init__(**kwargs)
-        if not isinstance(aws_conn_id, ArgNotSet):
-            warnings.warn(_DEPRECATION_MSG, AirflowProviderDeprecationWarning, stacklevel=3)
-            self.source_aws_conn_id = aws_conn_id
-        else:
-            self.source_aws_conn_id = source_aws_conn_id
-        self.dest_aws_conn_id = (
-            self.source_aws_conn_id if isinstance(dest_aws_conn_id, ArgNotSet) else dest_aws_conn_id
+        crawler_name: str,
+        poll_interval: int | None = None,
+        aws_conn_id: str = "aws_default",
+        waiter_delay: int = 5,
+        waiter_max_attempts: int = 1500,
+    ):
+        if poll_interval is not None:
+            warnings.warn(
+                "please use waiter_delay instead of poll_interval.",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+            waiter_delay = poll_interval or waiter_delay
+        super().__init__(
+            serialized_fields={"crawler_name": crawler_name},
+            waiter_name="crawler_ready",
+            waiter_args={"Name": crawler_name},
+            failure_message="Error while waiting for glue crawl to complete",
+            status_message="Status of glue crawl is",
+            status_queries=["Crawler.State", "Crawler.LastCrawl"],
+            return_value=None,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
+            aws_conn_id=aws_conn_id,
         )
+
+    def hook(self) -> AwsGenericHook:
+        return GlueCrawlerHook(aws_conn_id=self.aws_conn_id)
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 """This module contains Google Cloud Storage to S3 operator."""
 from __future__ import annotations
 
 import os
 import warnings
 from typing import TYPE_CHECKING, Sequence
 
-from airflow.exceptions import AirflowProviderDeprecationWarning
+from packaging.version import Version
+
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.s3 import S3Hook
 from airflow.providers.google.cloud.hooks.gcs import GCSHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -76,22 +78,25 @@
         account from the list granting this role to the originating account (templated).
     :param s3_acl_policy: Optional The string to specify the canned ACL policy for the
         object to be uploaded in S3
     :param keep_directory_structure: (Optional) When set to False the path of the file
          on the bucket is recreated within path passed in dest_s3_key.
     :param match_glob: (Optional) filters objects based on the glob pattern given by the string
         (e.g, ``'**/*/.json'``)
+    :param gcp_user_project: (Optional) The identifier of the Google Cloud project to bill for this request.
+        Required for Requester Pays buckets.
     """
 
     template_fields: Sequence[str] = (
         "bucket",
         "prefix",
         "delimiter",
         "dest_s3_key",
         "google_impersonation_chain",
+        "gcp_user_project",
     )
     ui_color = "#f0eee4"
 
     def __init__(
         self,
         *,
         bucket: str,
@@ -103,55 +108,78 @@
         dest_verify: str | bool | None = None,
         replace: bool = False,
         google_impersonation_chain: str | Sequence[str] | None = None,
         dest_s3_extra_args: dict | None = None,
         s3_acl_policy: str | None = None,
         keep_directory_structure: bool = True,
         match_glob: str | None = None,
+        gcp_user_project: str | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
 
         self.bucket = bucket
         self.prefix = prefix
-        if delimiter:
-            warnings.warn(
-                "Usage of 'delimiter' is deprecated, please use 'match_glob' instead",
-                AirflowProviderDeprecationWarning,
-                stacklevel=2,
-            )
-        self.delimiter = delimiter
         self.gcp_conn_id = gcp_conn_id
         self.dest_aws_conn_id = dest_aws_conn_id
         self.dest_s3_key = dest_s3_key
         self.dest_verify = dest_verify
         self.replace = replace
         self.google_impersonation_chain = google_impersonation_chain
         self.dest_s3_extra_args = dest_s3_extra_args or {}
         self.s3_acl_policy = s3_acl_policy
         self.keep_directory_structure = keep_directory_structure
+        try:
+            from airflow.providers.google import __version__
+
+            if Version(__version__) >= Version("10.3.0"):
+                self.__is_match_glob_supported = True
+            else:
+                self.__is_match_glob_supported = False
+        except ImportError:  # __version__ was added in 10.1.0, so this means it's < 10.3.0
+            self.__is_match_glob_supported = False
+        if self.__is_match_glob_supported:
+            if delimiter:
+                warnings.warn(
+                    "Usage of 'delimiter' is deprecated, please use 'match_glob' instead",
+                    AirflowProviderDeprecationWarning,
+                    stacklevel=2,
+                )
+        elif match_glob:
+            raise AirflowException(
+                "The 'match_glob' parameter requires 'apache-airflow-providers-google>=10.3.0'."
+            )
+        self.delimiter = delimiter
         self.match_glob = match_glob
+        self.gcp_user_project = gcp_user_project
 
     def execute(self, context: Context) -> list[str]:
         # list all files in an Google Cloud Storage bucket
-        hook = GCSHook(
+        gcs_hook = GCSHook(
             gcp_conn_id=self.gcp_conn_id,
             impersonation_chain=self.google_impersonation_chain,
         )
 
         self.log.info(
             "Getting list of the files. Bucket: %s; Delimiter: %s; Prefix: %s",
             self.bucket,
             self.delimiter,
             self.prefix,
         )
 
-        files = hook.list(
-            bucket_name=self.bucket, prefix=self.prefix, delimiter=self.delimiter, match_glob=self.match_glob
-        )
+        list_kwargs = {
+            "bucket_name": self.bucket,
+            "prefix": self.prefix,
+            "delimiter": self.delimiter,
+            "user_project": self.gcp_user_project,
+        }
+        if self.__is_match_glob_supported:
+            list_kwargs["match_glob"] = self.match_glob
+
+        gcs_files = gcs_hook.list(**list_kwargs)  # type: ignore
 
         s3_hook = S3Hook(
             aws_conn_id=self.dest_aws_conn_id, verify=self.dest_verify, extra_args=self.dest_s3_extra_args
         )
 
         if not self.keep_directory_structure and self.prefix:
             self.dest_s3_key = os.path.join(self.dest_s3_key, self.prefix)
@@ -169,28 +197,27 @@
             # look for the bucket and the prefix to avoid look into
             # parent directories/keys
             existing_files = s3_hook.list_keys(bucket_name, prefix=prefix)
             # in case that no files exists, return an empty array to avoid errors
             existing_files = existing_files if existing_files is not None else []
             # remove the prefix for the existing files to allow the match
             existing_files = [file.replace(prefix, "", 1) for file in existing_files]
-            files = list(set(files) - set(existing_files))
-
-        if files:
+            gcs_files = list(set(gcs_files) - set(existing_files))
 
-            for file in files:
-                with hook.provide_file(object_name=file, bucket_name=self.bucket) as local_tmp_file:
+        if gcs_files:
+            for file in gcs_files:
+                with gcs_hook.provide_file(
+                    object_name=file, bucket_name=self.bucket, user_project=self.gcp_user_project
+                ) as local_tmp_file:
                     dest_key = os.path.join(self.dest_s3_key, file)
                     self.log.info("Saving file to %s", dest_key)
-
                     s3_hook.load_file(
                         filename=local_tmp_file.name,
                         key=dest_key,
                         replace=self.replace,
                         acl_policy=self.s3_acl_policy,
                     )
-
-            self.log.info("All done, uploaded %d files to S3", len(files))
+            self.log.info("All done, uploaded %d files to S3", len(gcs_files))
         else:
             self.log.info("In sync, no files needed to be uploaded to S3")
 
-        return files
+        return gcs_files
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/athena.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/base.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/batch.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/ec2.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/ecs.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/eks.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/emr.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/glue.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/glue_crawler.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/step_function.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,54 +12,48 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-import warnings
-
-from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.amazon.aws.hooks.base_aws import AwsGenericHook
-from airflow.providers.amazon.aws.hooks.glue_crawler import GlueCrawlerHook
+from airflow.providers.amazon.aws.hooks.step_function import StepFunctionHook
 from airflow.providers.amazon.aws.triggers.base import AwsBaseWaiterTrigger
 
 
-class GlueCrawlerCompleteTrigger(AwsBaseWaiterTrigger):
+class StepFunctionsExecutionCompleteTrigger(AwsBaseWaiterTrigger):
     """
-    Watches for a glue crawl, triggers when it finishes.
+    Trigger to poll for the completion of a Step Functions execution.
 
-    :param crawler_name: name of the crawler to watch
-    :param poll_interval: The amount of time in seconds to wait between attempts.
+    :param execution_arn: ARN of the state machine to poll
+    :param waiter_delay: The amount of time in seconds to wait between attempts.
+    :param waiter_max_attempts: The maximum number of attempts to be made.
     :param aws_conn_id: The Airflow connection used for AWS credentials.
     """
 
     def __init__(
         self,
-        crawler_name: str,
-        poll_interval: int | None = None,
-        aws_conn_id: str = "aws_default",
-        waiter_delay: int = 5,
-        waiter_max_attempts: int = 1500,
-    ):
-        if poll_interval is not None:
-            warnings.warn(
-                "please use waiter_delay instead of poll_interval.",
-                AirflowProviderDeprecationWarning,
-                stacklevel=2,
-            )
-            waiter_delay = poll_interval or waiter_delay
+        *,
+        execution_arn: str,
+        waiter_delay: int = 60,
+        waiter_max_attempts: int = 30,
+        aws_conn_id: str | None = None,
+        region_name: str | None = None,
+    ) -> None:
+
         super().__init__(
-            serialized_fields={"crawler_name": crawler_name},
-            waiter_name="crawler_ready",
-            waiter_args={"Name": crawler_name},
-            failure_message="Error while waiting for glue crawl to complete",
-            status_message="Status of glue crawl is",
-            status_queries=["Crawler.State", "Crawler.LastCrawl"],
-            return_value=None,
+            serialized_fields={"execution_arn": execution_arn, "region_name": region_name},
+            waiter_name="step_function_succeeded",
+            waiter_args={"executionArn": execution_arn},
+            failure_message="Step function failed",
+            status_message="Status of step function execution is",
+            status_queries=["status", "error", "cause"],
+            return_key="execution_arn",
+            return_value=execution_arn,
             waiter_delay=waiter_delay,
             waiter_max_attempts=waiter_max_attempts,
             aws_conn_id=aws_conn_id,
         )
 
     def hook(self) -> AwsGenericHook:
-        return GlueCrawlerHook(aws_conn_id=self.aws_conn_id)
+        return StepFunctionHook(aws_conn_id=self.aws_conn_id, region_name=self.region_name)
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/rds.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/s3.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/task_log_fetcher.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/utils/waiter_with_logging.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/athena.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/athena.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/batch.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/batch.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/emr-containers.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/glue.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/glue.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/redshift.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/redshift.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/aws/waiters/stepfunctions.json` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/aws/waiters/stepfunctions.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.5.0rc1/airflow/providers/amazon/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-amazon",
         "name": "Amazon",
         "description": "Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).\n",
         "suspended": False,
         "versions": [
+            "8.5.0",
             "8.4.0",
             "8.3.1",
             "8.3.0",
             "8.2.0",
             "8.1.0",
             "8.0.0",
             "7.4.1",
@@ -712,14 +713,18 @@
                 "integration-name": "Amazon RDS",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.rds"],
             },
             {
                 "integration-name": "AWS Step Functions",
                 "python-modules": ["airflow.providers.amazon.aws.triggers.step_function"],
             },
+            {
+                "integration-name": "Amazon Simple Queue Service (SQS)",
+                "python-modules": ["airflow.providers.amazon.aws.triggers.sqs"],
+            },
         ],
         "transfers": [
             {
                 "source-integration-name": "Amazon DynamoDB",
                 "target-integration-name": "Amazon Simple Storage Service (S3)",
                 "how-to-guide": "/docs/apache-airflow-providers-amazon/transfer/dynamodb_to_s3.rst",
                 "python-module": "airflow.providers.amazon.aws.transfers.dynamodb_to_s3",
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.4.0rc1
+Version: 8.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -35,14 +35,15 @@
 Provides-Extra: exasol
 Provides-Extra: ftp
 Provides-Extra: google
 Provides-Extra: http
 Provides-Extra: imap
 Provides-Extra: microsoft.azure
 Provides-Extra: mongo
+Provides-Extra: openlineage
 Provides-Extra: salesforce
 Provides-Extra: ssh
 Provides-Extra: pandas
 Provides-Extra: aiobotocore
 License-File: LICENSE
 License-File: NOTICE
 
@@ -80,28 +81,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.4.0rc1``
+Release: ``8.5.0rc1``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``amazon`` provider. All classes for this provider package
 are in ``airflow.providers.amazon`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -153,13 +154,14 @@
 `apache-airflow-providers-exasol <https://airflow.apache.org/docs/apache-airflow-providers-exasol>`_                    ``exasol``
 `apache-airflow-providers-ftp <https://airflow.apache.org/docs/apache-airflow-providers-ftp>`_                          ``ftp``
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_                    ``google``
 `apache-airflow-providers-http <https://airflow.apache.org/docs/apache-airflow-providers-http>`_                        ``http``
 `apache-airflow-providers-imap <https://airflow.apache.org/docs/apache-airflow-providers-imap>`_                        ``imap``
 `apache-airflow-providers-microsoft-azure <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure>`_  ``microsoft.azure``
 `apache-airflow-providers-mongo <https://airflow.apache.org/docs/apache-airflow-providers-mongo>`_                      ``mongo``
+`apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_          ``openlineage``
 `apache-airflow-providers-salesforce <https://airflow.apache.org/docs/apache-airflow-providers-salesforce>`_            ``salesforce``
 `apache-airflow-providers-ssh <https://airflow.apache.org/docs/apache-airflow-providers-ssh>`_                          ``ssh``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/changelog.html>`_.
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -141,22 +141,24 @@
 airflow/providers/amazon/aws/triggers/emr.py
 airflow/providers/amazon/aws/triggers/glue.py
 airflow/providers/amazon/aws/triggers/glue_crawler.py
 airflow/providers/amazon/aws/triggers/rds.py
 airflow/providers/amazon/aws/triggers/redshift_cluster.py
 airflow/providers/amazon/aws/triggers/s3.py
 airflow/providers/amazon/aws/triggers/sagemaker.py
+airflow/providers/amazon/aws/triggers/sqs.py
 airflow/providers/amazon/aws/triggers/step_function.py
 airflow/providers/amazon/aws/utils/__init__.py
 airflow/providers/amazon/aws/utils/connection_wrapper.py
 airflow/providers/amazon/aws/utils/eks_get_token.py
 airflow/providers/amazon/aws/utils/emailer.py
 airflow/providers/amazon/aws/utils/rds.py
 airflow/providers/amazon/aws/utils/redshift.py
 airflow/providers/amazon/aws/utils/sagemaker.py
+airflow/providers/amazon/aws/utils/sqs.py
 airflow/providers/amazon/aws/utils/tags.py
 airflow/providers/amazon/aws/utils/task_log_fetcher.py
 airflow/providers/amazon/aws/utils/waiter.py
 airflow/providers/amazon/aws/utils/waiter_with_logging.py
 airflow/providers/amazon/aws/waiters/__init__.py
 airflow/providers/amazon/aws/waiters/appflow.json
 airflow/providers/amazon/aws/waiters/athena.json
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.5.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 
 [microsoft.azure]
 apache-airflow-providers-microsoft-azure
 
 [mongo]
 apache-airflow-providers-mongo
 
+[openlineage]
+apache-airflow-providers-openlineage
+
 [pandas]
 pandas>=0.17.1
 
 [salesforce]
 apache-airflow-providers-salesforce
 
 [ssh]
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/pyproject.toml` & `apache-airflow-providers-amazon-8.5.0rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
     "test_*.py",
+    "example_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
 required-imports = ["from __future__ import annotations"]
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/setup.cfg` & `apache-airflow-providers-amazon-8.5.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.4.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.5.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-amazon-8.4.0rc1/setup.py` & `apache-airflow-providers-amazon-8.5.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-amazon package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "8.4.0"
+version = "8.5.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-amazon setup."""
     setup(
         version=version,
         extras_require={
@@ -40,14 +40,15 @@
             "exasol": ["apache-airflow-providers-exasol"],
             "ftp": ["apache-airflow-providers-ftp"],
             "google": ["apache-airflow-providers-google"],
             "http": ["apache-airflow-providers-http"],
             "imap": ["apache-airflow-providers-imap"],
             "microsoft.azure": ["apache-airflow-providers-microsoft-azure"],
             "mongo": ["apache-airflow-providers-mongo"],
+            "openlineage": ["apache-airflow-providers-openlineage"],
             "salesforce": ["apache-airflow-providers-salesforce"],
             "ssh": ["apache-airflow-providers-ssh"],
             "pandas": ["pandas>=0.17.1"],
             "aiobotocore": ["aiobotocore[boto3]>=2.2.0"],
         },
         packages=find_namespace_packages(
             include=[
```

