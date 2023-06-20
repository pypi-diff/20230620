# Comparing `tmp/apache-airflow-providers-amazon-8.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-amazon-8.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-amazon-8.1.0rc1.tar", last modified: Tue May 16 15:52:50 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-amazon-8.1.0rc2.tar", last modified: Fri May 19 17:51:27 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.1.0rc1.tar` & `apache-airflow-providers-amazon-8.1.0rc2.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-05-16 15:52:48.000000 apache-airflow-providers-amazon-8.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    59663 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    57842 2023-05-16 15:52:48.000000 apache-airflow-providers-amazon-8.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12240 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    45981 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    20625 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)     9697 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7921 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    20465 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    14759 2023-04-30 16:30:42.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     4823 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13287 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     7072 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    43170 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-05-04 19:22:39.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2943 2023-05-04 19:17:30.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     2401 2023-05-04 19:17:30.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)    16635 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    29018 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    31814 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    53336 2023-05-12 22:41:38.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    29868 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    29124 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5559 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    55195 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-05-05 08:06:03.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15628 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     3658 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    19390 2023-05-04 19:17:30.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3332 2023-04-30 16:30:42.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2848 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     7703 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     7676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6007 2023-05-16 07:40:59.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8286 2023-05-05 08:06:03.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8475 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3006 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/ec2.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3853 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20488 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)     1853 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json
--rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)      430 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/emr-serverless.json
--rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)     2699 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json
--rw-r--r--   0 root         (0) root         (0)    36891 2023-05-16 15:52:48.000000 apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    59663 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7463 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-amazon-8.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2106 2023-05-16 15:52:50.000000 apache-airflow-providers-amazon-8.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2363 2023-05-16 15:52:48.000000 apache-airflow-providers-amazon-8.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.1.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-05-19 17:51:25.000000 apache-airflow-providers-amazon-8.1.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.1.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    60089 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    58268 2023-05-19 17:51:25.000000 apache-airflow-providers-amazon-8.1.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 11:58:20.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12240 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    46038 2023-05-18 08:56:29.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    20625 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)     9697 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7921 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    20465 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    14759 2023-04-30 16:30:42.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13287 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     7072 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    43170 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-05-04 19:22:39.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-05-04 19:17:30.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-05-04 19:17:30.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    16635 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    29018 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    31814 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    53336 2023-05-12 22:41:38.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    29868 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    29124 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    55195 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     4583 2023-05-05 08:06:03.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15628 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     4437 2023-05-19 11:18:18.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    19390 2023-05-04 19:17:30.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3332 2023-04-30 16:30:42.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     7845 2023-05-18 08:56:29.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     7676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6007 2023-05-16 07:40:59.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8286 2023-05-05 08:06:03.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8475 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-05-15 07:14:11.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/triggers/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3853 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/triggers/sagemaker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20488 2023-05-03 19:47:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/waiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/dynamodb.json
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      430 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-05-12 08:38:07.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/sagemaker.json
+-rw-r--r--   0 root         (0) root         (0)    36891 2023-05-19 17:51:25.000000 apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    60089 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7463 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-amazon-8.1.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-05-19 17:51:27.000000 apache-airflow-providers-amazon-8.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-05-19 17:51:25.000000 apache-airflow-providers-amazon-8.1.0rc2/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/LICENSE` & `apache-airflow-providers-amazon-8.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/MANIFEST.in` & `apache-airflow-providers-amazon-8.1.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/PKG-INFO` & `apache-airflow-providers-amazon-8.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.1.0rc1
+Version: 8.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.1.0/
@@ -60,15 +60,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.1.0rc1``
+Release: ``8.1.0rc2``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
@@ -197,23 +197,29 @@
 * ``Add tags param in RedshiftCreateClusterSnapshotOperator (#31006)``
 * ``improve/fix glue job logs printing (#30886)``
 * ``Import aiobotocore only if deferrable is true (#31094)``
 * ``Update return types of 'get_key' methods on 'S3Hook' (#30923)``
 * ``Support 'shareIdentifier' in BatchOperator (#30829)``
 * ``BaseAWS - Override client when resource_type is user to get custom waiters (#30897)``
 * ``Add future-compatible mongo Hook typing (#31289)``
+* ``Handle temporary credentials when resource_type is used to get custom waiters (#31333)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Move TaskInstanceKey to a separate file (#31033)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)``
    * ``Revert "DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)" (#31139)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Bring back detection of implicit single-line string concatenation (#31270)``
+   * ``Fix AWS system test example_dynamodb (#31395)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Fix AWS system test example_dynamodb_to_s3 (#31362)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 8.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/README.rst` & `apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,52 @@
+Metadata-Version: 2.1
+Name: apache-airflow-providers-amazon
+Version: 8.1.0rc2
+Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
+Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
+Author: Apache Software Foundation
+Author-email: dev@airflow.apache.org
+License: Apache License 2.0
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.1.0/
+Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
+Project-URL: Source Code, https://github.com/apache/airflow
+Project-URL: Slack Chat, https://s.apache.org/airflow-slack
+Project-URL: Twitter, https://twitter.com/ApacheAirflow
+Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Framework :: Apache Airflow
+Classifier: Framework :: Apache Airflow :: Provider
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: System :: Monitoring
+Requires-Python: ~=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: apache.hive
+Provides-Extra: cncf.kubernetes
+Provides-Extra: common.sql
+Provides-Extra: exasol
+Provides-Extra: ftp
+Provides-Extra: google
+Provides-Extra: imap
+Provides-Extra: mongo
+Provides-Extra: salesforce
+Provides-Extra: ssh
+Provides-Extra: pandas
+Provides-Extra: aiobotocore
+License-File: LICENSE
+License-File: NOTICE
+
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
@@ -15,15 +60,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.1.0rc1``
+Release: ``8.1.0rc2``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
@@ -152,23 +197,29 @@
 * ``Add tags param in RedshiftCreateClusterSnapshotOperator (#31006)``
 * ``improve/fix glue job logs printing (#30886)``
 * ``Import aiobotocore only if deferrable is true (#31094)``
 * ``Update return types of 'get_key' methods on 'S3Hook' (#30923)``
 * ``Support 'shareIdentifier' in BatchOperator (#30829)``
 * ``BaseAWS - Override client when resource_type is user to get custom waiters (#30897)``
 * ``Add future-compatible mongo Hook typing (#31289)``
+* ``Handle temporary credentials when resource_type is used to get custom waiters (#31333)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Move TaskInstanceKey to a separate file (#31033)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)``
    * ``Revert "DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)" (#31139)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Bring back detection of implicit single-line string concatenation (#31270)``
+   * ``Fix AWS system test example_dynamodb (#31395)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Fix AWS system test example_dynamodb_to_s3 (#31362)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 8.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -849,14 +849,15 @@
             if self.resource_type:
                 credentials = self.get_credentials()
                 client = boto3.client(
                     self.resource_type,
                     region_name=self.region_name,
                     aws_access_key_id=credentials.access_key,
                     aws_secret_access_key=credentials.secret_key,
+                    aws_session_token=credentials.token,
                 )
 
             # Technically if waiter_name is in custom_waiters then self.waiter_path must
             # exist but MyPy doesn't like the fact that self.waiter_path could be None.
             with open(self.waiter_path) as config_file:
                 config = json.loads(config_file.read())
```

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,36 +12,53 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.compat.functools import cached_property
 from airflow.providers.amazon.aws.hooks.dynamodb import DynamoDBHook
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class DynamoDBValueSensor(BaseSensorOperator):
     """
     Waits for an attribute value to be present for an item in a DynamoDB table.
 
+    .. seealso::
+        For more information on how to use this sensor, take a look at the guide:
+        :ref:`howto/sensor:DynamoDBValueSensor`
+
+    :param table_name: DynamoDB table name
     :param partition_key_name: DynamoDB partition key name
     :param partition_key_value: DynamoDB partition key value
     :param attribute_name: DynamoDB attribute name
     :param attribute_value: DynamoDB attribute value
     :param sort_key_name: (optional) DynamoDB sort key name
     :param sort_key_value: (optional) DynamoDB sort key value
+    :param aws_conn_id: aws connection to use
+    :param region_name: aws region to use
     """
 
+    template_fields: Sequence[str] = (
+        "table_name",
+        "partition_key_name",
+        "partition_key_value",
+        "attribute_name",
+        "attribute_value",
+        "sort_key_name",
+        "sort_key_value",
+    )
+
     def __init__(
         self,
         table_name: str,
         partition_key_name: str,
         partition_key_value: str,
         attribute_name: str,
         attribute_value: str,
```

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,17 +93,22 @@
      the Unix epoch. The table export will be a snapshot of the table's state at this point in time.
     :param export_format: The format for the exported data. Valid values for ExportFormat are DYNAMODB_JSON
      or ION.
     """
 
     template_fields: Sequence[str] = (
         *AwsToAwsBaseOperator.template_fields,
+        "dynamodb_table_name",
         "s3_bucket_name",
+        "file_size",
+        "dynamodb_scan_kwargs",
         "s3_key_prefix",
-        "dynamodb_table_name",
+        "process_func",
+        "export_time",
+        "export_format",
     )
 
     template_fields_renderers = {
         "dynamodb_scan_kwargs": "json",
     }
 
     def __init__(
@@ -125,17 +130,14 @@
         self.dynamodb_table_name = dynamodb_table_name
         self.dynamodb_scan_kwargs = dynamodb_scan_kwargs
         self.s3_bucket_name = s3_bucket_name
         self.s3_key_prefix = s3_key_prefix
         self.export_time = export_time
         self.export_format = export_format
 
-        if self.export_time and self.export_time > datetime.now():
-            raise ValueError("The export_time parameter cannot be a future time.")
-
     @cached_property
     def hook(self):
         """Create DynamoDBHook"""
         return DynamoDBHook(aws_conn_id=self.source_aws_conn_id)
 
     def execute(self, context: Context) -> None:
         if self.export_time:
@@ -144,14 +146,17 @@
             self._export_entire_data()
 
     def _export_table_to_point_in_time(self):
         """
         Export data from start of epoc till `export_time`. Table export will be a snapshot of the table's
          state at this point in time.
         """
+        if self.export_time and self.export_time > datetime.now(self.export_time.tzinfo):
+            raise ValueError("The export_time parameter cannot be a future time.")
+
         client = self.hook.conn.meta.client
         table_description = client.describe_table(TableName=self.dynamodb_table_name)
         response = client.export_table_to_point_in_time(
             TableArn=table_description.get("Table", {}).get("TableArn"),
             ExportTime=self.export_time,
             S3Bucket=self.s3_bucket_name,
             S3Prefix=self.s3_key_prefix,
@@ -159,15 +164,15 @@
         )
         waiter = self.hook.get_waiter("export_table")
         export_arn = response.get("ExportDescription", {}).get("ExportArn")
         waiter.wait(ExportArn=export_arn)
 
     def _export_entire_data(self):
         """Export all data from the table."""
-        table = self.hook.get_conn().Table(self.dynamodb_table_name)
+        table = self.hook.conn.Table(self.dynamodb_table_name)
         scan_kwargs = copy(self.dynamodb_scan_kwargs) if self.dynamodb_scan_kwargs else {}
         err = None
         f: IO[Any]
         with NamedTemporaryFile() as f:
             try:
                 f = self._scan_dynamodb_and_upload_to_s3(f, scan_kwargs, table)
             except Exception as e:
```

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/ec2.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/triggers/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/triggers/sagemaker.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/triggers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/dynamodb.json` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/dynamodb.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/aws/waiters/sagemaker.json` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/aws/waiters/sagemaker.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.1.0rc2/airflow/providers/amazon/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.1.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,7 @@
-Metadata-Version: 2.1
-Name: apache-airflow-providers-amazon
-Version: 8.1.0rc1
-Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
-Home-page: https://airflow.apache.org/
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Author: Apache Software Foundation
-Author-email: dev@airflow.apache.org
-License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.1.0/
-Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Source Code, https://github.com/apache/airflow
-Project-URL: Slack Chat, https://s.apache.org/airflow-slack
-Project-URL: Twitter, https://twitter.com/ApacheAirflow
-Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Framework :: Apache Airflow
-Classifier: Framework :: Apache Airflow :: Provider
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: apache.hive
-Provides-Extra: cncf.kubernetes
-Provides-Extra: common.sql
-Provides-Extra: exasol
-Provides-Extra: ftp
-Provides-Extra: google
-Provides-Extra: imap
-Provides-Extra: mongo
-Provides-Extra: salesforce
-Provides-Extra: ssh
-Provides-Extra: pandas
-Provides-Extra: aiobotocore
-License-File: LICENSE
-License-File: NOTICE
-
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
@@ -60,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.1.0rc1``
+Release: ``8.1.0rc2``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
@@ -197,23 +152,29 @@
 * ``Add tags param in RedshiftCreateClusterSnapshotOperator (#31006)``
 * ``improve/fix glue job logs printing (#30886)``
 * ``Import aiobotocore only if deferrable is true (#31094)``
 * ``Update return types of 'get_key' methods on 'S3Hook' (#30923)``
 * ``Support 'shareIdentifier' in BatchOperator (#30829)``
 * ``BaseAWS - Override client when resource_type is user to get custom waiters (#30897)``
 * ``Add future-compatible mongo Hook typing (#31289)``
+* ``Handle temporary credentials when resource_type is used to get custom waiters (#31333)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Move TaskInstanceKey to a separate file (#31033)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)``
    * ``Revert "DynamoDBToS3Operator - Add feature to export table to a point in time (#30501)" (#31139)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Bring back detection of implicit single-line string concatenation (#31270)``
+   * ``Fix AWS system test example_dynamodb (#31395)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Fix AWS system test example_dynamodb_to_s3 (#31362)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 8.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.1.0rc2/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/pyproject.toml` & `apache-airflow-providers-amazon-8.1.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     # implicit single-line string concatenation
     "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
+    # "D400", WIP: see #31135
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
     "D403",
     "D412",
     "D419"
 ]
 extend-ignore = [
```

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/setup.cfg` & `apache-airflow-providers-amazon-8.1.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -63,10 +63,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.amazon.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.amazon
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-amazon-8.1.0rc1/setup.py` & `apache-airflow-providers-amazon-8.1.0rc2/setup.py`

 * *Files identical despite different names*

