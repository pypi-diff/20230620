# Comparing `tmp/localstack-core-2.1.1.dev20230619173831.tar.gz` & `tmp/localstack-core-2.1.1.dev20230620171514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230619173831.tar", last modified: Mon Jun 19 17:38:38 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230620171514.tar", last modified: Tue Jun 20 17:15:22 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230619173831.tar` & `localstack-core-2.1.1.dev20230620171514.tar`

### file list

```diff
@@ -1,856 +1,856 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.691989 localstack-core-2.1.1.dev20230619173831/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-19 17:38:38.691989 localstack-core-2.1.1.dev20230619173831/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-19 17:38:31.000000 localstack-core-2.1.1.dev20230619173831/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.595989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   759418 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   133075 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.599989 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.603989 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.603989 localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-19 17:02:15.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.603989 localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.603989 localstack-core-2.1.1.dev20230619173831/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.603989 localstack-core-2.1.1.dev20230619173831/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.603989 localstack-core-2.1.1.dev20230619173831/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.603989 localstack-core-2.1.1.dev20230619173831/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.607989 localstack-core-2.1.1.dev20230619173831/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.607989 localstack-core-2.1.1.dev20230619173831/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.607989 localstack-core-2.1.1.dev20230619173831/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.607989 localstack-core-2.1.1.dev20230619173831/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.607989 localstack-core-2.1.1.dev20230619173831/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.607989 localstack-core-2.1.1.dev20230619173831/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.611989 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    63526 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38422 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14794 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10909 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.611989 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.611989 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.611989 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.615989 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.615989 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.615989 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65108 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33005 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20991 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7434 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2190 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21924 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2949 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3188 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9196 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28213 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3327 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4787 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2640 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13639 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6708 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8678 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5134 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3927 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5754 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5500 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.619989 localstack-core-2.1.1.dev20230619173831/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.623989 localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.623989 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59738 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.623989 localstack-core-2.1.1.dev20230619173831/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.623989 localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.623989 localstack-core-2.1.1.dev20230619173831/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.623989 localstack-core-2.1.1.dev20230619173831/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.623989 localstack-core-2.1.1.dev20230619173831/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.623989 localstack-core-2.1.1.dev20230619173831/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.623989 localstack-core-2.1.1.dev20230619173831/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43901 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.627989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.631989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.631989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.631989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.635989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.635989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.635989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.635989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.635989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.635989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.635989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.635989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.643989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.643989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.643989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.643989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.643989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.643989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.643989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.651989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.659989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.659989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.659989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.659989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.659989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.663989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.663989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.663989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.663989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4358 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2035 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4960 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4363 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3053 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4242 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3566 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.667989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.667989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.667989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.667989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.667989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1694 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.667989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.671989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3143 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.671989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.671989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.671989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.671989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.671989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31120 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.671989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.675989 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12321 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.675989 localstack-core-2.1.1.dev20230619173831/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.675989 localstack-core-2.1.1.dev20230619173831/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.675989 localstack-core-2.1.1.dev20230619173831/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.675989 localstack-core-2.1.1.dev20230619173831/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.679989 localstack-core-2.1.1.dev20230619173831/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.679989 localstack-core-2.1.1.dev20230619173831/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.679989 localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.679989 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69752 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.679989 localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.683989 localstack-core-2.1.1.dev20230619173831/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.687989 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.687989 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.687989 localstack-core-2.1.1.dev20230619173831/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.687989 localstack-core-2.1.1.dev20230619173831/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.687989 localstack-core-2.1.1.dev20230619173831/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.687989 localstack-core-2.1.1.dev20230619173831/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 17:38:38.691989 localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-19 17:38:38.000000 localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38094 2023-06-19 17:38:38.000000 localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-19 17:38:38.000000 localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-19 17:38:38.000000 localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-19 17:38:35.000000 localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-19 17:38:35.000000 localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-19 17:38:38.000000 localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-19 17:38:38.000000 localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-19 17:38:38.691989 localstack-core-2.1.1.dev20230619173831/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-19 17:02:16.000000 localstack-core-2.1.1.dev20230619173831/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.247183 localstack-core-2.1.1.dev20230620171514/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-20 17:15:22.247183 localstack-core-2.1.1.dev20230620171514/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.095184 localstack-core-2.1.1.dev20230620171514/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-20 17:15:14.000000 localstack-core-2.1.1.dev20230620171514/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   759418 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.099184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   133075 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.103184 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.107184 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.107184 localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.107184 localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.107184 localstack-core-2.1.1.dev20230620171514/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.107184 localstack-core-2.1.1.dev20230620171514/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.107184 localstack-core-2.1.1.dev20230620171514/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.147184 localstack-core-2.1.1.dev20230620171514/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.147184 localstack-core-2.1.1.dev20230620171514/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.147184 localstack-core-2.1.1.dev20230620171514/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.151184 localstack-core-2.1.1.dev20230620171514/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.151184 localstack-core-2.1.1.dev20230620171514/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.151184 localstack-core-2.1.1.dev20230620171514/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.151184 localstack-core-2.1.1.dev20230620171514/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.151184 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    63526 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38422 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14794 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10909 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.155184 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.155184 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.155184 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.155184 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.163184 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8939 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.163184 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    66262 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.163184 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33198 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21664 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7543 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2283 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5799 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21924 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2949 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3340 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9352 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28370 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3420 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4787 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2806 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3727 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13743 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6906 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8951 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5130 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3927 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5875 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5500 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.163184 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.167183 localstack-core-2.1.1.dev20230620171514/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.167183 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.167183 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.171184 localstack-core-2.1.1.dev20230620171514/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59738 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.175184 localstack-core-2.1.1.dev20230620171514/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.179184 localstack-core-2.1.1.dev20230620171514/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.179184 localstack-core-2.1.1.dev20230620171514/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.179184 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.179184 localstack-core-2.1.1.dev20230620171514/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.179184 localstack-core-2.1.1.dev20230620171514/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.183184 localstack-core-2.1.1.dev20230620171514/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.183184 localstack-core-2.1.1.dev20230620171514/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43901 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.183184 localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.183184 localstack-core-2.1.1.dev20230620171514/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.183184 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.187183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.187183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.187183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.187183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.187183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.187183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.191183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.191183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.191183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.191183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.191183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.191183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.191183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.191183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.199184 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.199184 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.199184 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.199184 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.199184 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.199184 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.207183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.211183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.215183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.215183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.215183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.215183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.215183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.219183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.219183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.219183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.223183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4358 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2035 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4960 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4363 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3053 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4242 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3566 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.223183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.223183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.223183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.223183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.227183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1694 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.227183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.227183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3143 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.227183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.227183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.227183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.227183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.227183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31120 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12321 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.235183 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69752 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.239183 localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.243183 localstack-core-2.1.1.dev20230620171514/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.243183 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.247183 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.247183 localstack-core-2.1.1.dev20230620171514/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.247183 localstack-core-2.1.1.dev20230620171514/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.247183 localstack-core-2.1.1.dev20230620171514/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.247183 localstack-core-2.1.1.dev20230620171514/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 17:15:22.247183 localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-20 17:15:21.000000 localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38094 2023-06-20 17:15:22.000000 localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-20 17:15:21.000000 localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-20 17:15:21.000000 localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-20 17:15:18.000000 localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-20 17:15:18.000000 localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-20 17:15:21.000000 localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-20 17:15:21.000000 localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-20 17:15:22.247183 localstack-core-2.1.1.dev20230620171514/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-20 16:42:00.000000 localstack-core-2.1.1.dev20230620171514/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230619173831/LICENSE.txt` & `localstack-core-2.1.1.dev20230620171514/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/Makefile` & `localstack-core-2.1.1.dev20230620171514/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/PKG-INFO` & `localstack-core-2.1.1.dev20230620171514/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230619173831
+Version: 2.1.1.dev20230620171514
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230619173831/README.md` & `localstack-core-2.1.1.dev20230620171514/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/bin/localstack` & `localstack-core-2.1.1.dev20230620171514/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230620171514/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230620171514/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230620171514/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230620171514/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230620171514/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230620171514/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230620171514/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/config.py` & `localstack-core-2.1.1.dev20230620171514/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/constants.py` & `localstack-core-2.1.1.dev20230620171514/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230620171514/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230620171514/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230620171514/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/client.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/request.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/response.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/http/router.py` & `localstack-core-2.1.1.dev20230620171514/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230620171514/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230620171514/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230620171514/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230620171514/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230620171514/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230620171514/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/packages/ffmpeg.py` & `localstack-core-2.1.1.dev20230620171514/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230620171514/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/plugins.py` & `localstack-core-2.1.1.dev20230620171514/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230620171514/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230620171514/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230620171514/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230620171514/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230620171514/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/cfn_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 import json
 from typing import Callable
 
 from localstack.utils.objects import recurse_object
 
 
 def rename_params(func, rename_map):
-    def do_rename(params, **kwargs):
-        values = func(params, **kwargs) if func else params
+    def do_rename(params, logical_resource_id, *args, **kwargs):
+        values = func(params, logical_resource_id, *args, **kwargs) if func else params
         for old_param, new_param in rename_map.items():
             values[new_param] = values.pop(old_param, None)
         return values
 
     return do_rename
 
 
-def lambda_add_tags(func):
-    return lambda params, **kwargs: add_tags(func(params, **kwargs))
-
-
 def lambda_convert_types(func, types):
-    return lambda params, **kwargs: convert_types(func(params, **kwargs), types)
+    return lambda params, logical_resource_id, *args, **kwargs: convert_types(
+        func(params, *args, **kwargs), types
+    )
 
 
 def lambda_to_json(attr):
-    return lambda params, **kwargs: json.dumps(params[attr])
-
-
-def add_tags(obj, tags=[]):
-    tags = tags or []
-    obj["tags"] = obj.get("tags") or []
-    obj["tags"].extend(tags)
-    return obj
+    return lambda params, logical_resource_id, *args, **kwargs: json.dumps(params[attr])
 
 
 def lambda_rename_attributes(attrs, func=None):
     def recurse(o, path):
         if isinstance(o, dict):
             for k in list(o.keys()):
                 for a in attrs.keys():
                     if k == a:
                         o[attrs[k]] = o.pop(k)
         return o
 
-    func = func or (lambda x, **kwargs: x)
-    return lambda params, **kwargs: recurse_object(func(params, **kwargs), recurse)
+    func = func or (lambda x, logical_resource_id, *args, **kwargs: x)
+    return lambda params, logical_resource_id, *args, **kwargs: recurse_object(
+        func(params, logical_resource_id, *args, **kwargs), recurse
+    )
 
 
 def convert_types(obj, types):
     def fix_types(key, type_class):
         def recurse(o, path):
             if isinstance(o, dict):
                 for k, v in dict(o).items():
@@ -62,15 +55,15 @@
         fix_types(key, type_class)
     return obj
 
 
 def get_tags_param(resource_type: str) -> Callable:
     """Return a tag parameters creation function for the given resource type"""
 
-    def _param(params, **kwargs):
+    def _param(params, logical_resource_id, *args, **kwargs):
         tags = params.get("Tags")
         if not tags:
             return None
 
         return [{"ResourceType": resource_type, "Tags": tags}]
 
     return _param
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/deployment_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 # placeholders
 PLACEHOLDER_AWS_NO_VALUE = "__aws_no_value__"
 
 LOG = logging.getLogger(__name__)
 
 
 def dump_json_params(param_func=None, *param_names):
-    def replace(params, **kwargs):
-        result = param_func(params, **kwargs) if param_func else params
+    def replace(params, logical_resource_id, *args, **kwargs):
+        result = param_func(params, logical_resource_id, *args, **kwargs) if param_func else params
         for name in param_names:
             if isinstance(result.get(name), (dict, list)):
                 # Fix for https://github.com/localstack/localstack/issues/2022
                 # Convert any date instances to date strings, etc, Version: "2012-10-17"
                 param_value = common.json_safe(result[name])
                 result[name] = json.dumps(param_value)
         return result
 
     return replace
 
 
 def param_defaults(param_func, defaults):
-    def replace(params, **kwargs):
-        result = param_func(params, **kwargs)
+    def replace(properties: dict, logical_resource_id: str, *args, **kwargs):
+        result = param_func(properties, logical_resource_id, *args, **kwargs)
         for key, value in defaults.items():
             if result.get(key) in ["", None]:
                 result[key] = value
         return result
 
     return replace
 
@@ -58,81 +58,84 @@
         return o
 
     result = common.recurse_object(params, remove_nones)
     return result
 
 
 def params_list_to_dict(param_name, key_attr_name="Key", value_attr_name="Value"):
-    def do_replace(params, **kwargs):
+    def do_replace(params, logical_resource_id, *args, **kwargs):
         result = {}
         for entry in params.get(param_name, []):
             key = entry[key_attr_name]
             value = entry[value_attr_name]
             result[key] = value
         return result
 
     return do_replace
 
 
 def lambda_keys_to_lower(key=None, skip_children_of: List[str] = None):
-    return lambda params, **kwargs: common.keys_to_lower(
+    return lambda params, logical_resource_id, *args, **kwargs: common.keys_to_lower(
         obj=(params.get(key) if key else params), skip_children_of=skip_children_of
     )
 
 
 def merge_parameters(func1, func2):
-    return lambda params, **kwargs: common.merge_dicts(
-        func1(params, **kwargs), func2(params, **kwargs)
+    return lambda properties, logical_resource_id, *args, **kwargs: common.merge_dicts(
+        func1(properties, logical_resource_id, *args, **kwargs),
+        func2(properties, logical_resource_id, *args, **kwargs),
     )
 
 
 def str_or_none(o):
     return o if o is None else json.dumps(o) if isinstance(o, (dict, list)) else str(o)
 
 
 def params_dict_to_list(param_name, key_attr_name="Key", value_attr_name="Value", wrapper=None):
-    def do_replace(params, **kwargs):
+    def do_replace(params, logical_resource_id, *args, **kwargs):
         result = []
         for key, value in params.get(param_name, {}).items():
             result.append({key_attr_name: key, value_attr_name: value})
         if wrapper:
             result = {wrapper: result}
         return result
 
     return do_replace
 
 
 def params_select_attributes(*attrs):
-    def do_select(params, **kwargs):
+    def do_select(params, logical_resource_id, *args, **kwargs):
         result = {}
         for attr in attrs:
             if params.get(attr) is not None:
                 result[attr] = str_or_none(params.get(attr))
         return result
 
     return do_select
 
 
 def param_json_to_str(name):
-    def _convert(params, **kwargs):
+    def _convert(params, logical_resource_id, *args, **kwargs):
         result = params.get(name)
         if result:
             result = json.dumps(result)
         return result
 
     return _convert
 
 
 def lambda_select_params(*selected):
     # TODO: remove and merge with function below
     return select_parameters(*selected)
 
 
 def select_parameters(*param_names):
-    return lambda params, **kwargs: select_attributes(params, param_names)
+    return lambda properties, logical_resource_id, *args, **kwargs: select_attributes(
+        properties, param_names
+    )
 
 
 def is_none_or_empty_value(value):
     return not value or value == PLACEHOLDER_AWS_NO_VALUE
 
 
 def generate_default_name(stack_name: str, logical_resource_id: str):
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,28 +66,46 @@
 # - resource_props
 # - stack_name
 # - resources
 # - resource_id
 ResourceProp = str | Callable[[dict, str, dict, str], dict]
 ResourceDefinition = dict[str, ResourceProp]
 
+# - logical_resource_id
+# - resource
+# - stack_name
+FunctionFuncSignature = Callable[[str, dict, str], Any]
+# - resource_id
+# - resources
+# - resource_type
+# - func
+# - stack_name
+FunctionFuncSignatureLegacy = Callable[[str, dict[str, dict], str, Any, str], Any]
+
+# - resource_props
+# - logical_resource_id
+# - resource
+# - stack_name
+ParamsFuncSignature = Callable[[dict, str, dict, str], dict]
+# - resource_props
+# - stack_name
+# - resources
+# - resource_id
+ParamsFuncSignatureLegacy = Callable[[dict, str, dict[str, dict], str], dict]
+
+# either a dictionary of strings to
+# - strings, or
+# - instances of the parameter function (current or legacy)
+ParamsDefinition = dict[str, str | ParamsFuncSignature | ParamsFuncSignatureLegacy]
+
 
 class FuncDetailsValue(TypedDict):
-    # Callable here takes the arguments:
-    # - logical_resource_id
-    # - resource
-    # - stack_name
-    function: str | Callable[[str, dict, str], Any]
+    function: str | FunctionFuncSignature | FunctionFuncSignatureLegacy
     """Either an api method to call directly with `parameters` or a callable to directly invoke"""
-    # Callable here takes the arguments:
-    # - resource_props
-    # - stack_name
-    # - resources
-    # - resource_id
-    parameters: Optional[ResourceDefinition | Callable[[dict, str, list[dict], str], dict]]
+    parameters: Optional[ParamsDefinition | ParamsFuncSignature | ParamsFuncSignatureLegacy]
     """arguments to the function, or a function that generates the arguments to the function"""
     # Callable here takes the arguments
     # - result
     # - resource_id
     # - resources
     # - resource_type
     result_handler: Optional[Callable[[dict, str, list[dict], str], None]]
@@ -804,15 +822,14 @@
     )
     func_details = func_details[action_name]
     func_details = func_details if isinstance(func_details, list) else [func_details]
     results = []
     for func in func_details:
         result = None
         executed = False
-        # TODO(srw) 3 - callable function
         if callable(func.get("function")):
             sig = inspect.signature(func["function"])
             if "logical_resource_id" in sig.parameters:
                 result = func["function"](resource_id, resources[resource_id], stack_name)
             else:
                 result = func["function"](resource_id, resources, resource_type, func, stack_name)
             results.append(result)
@@ -889,28 +906,34 @@
 def resolve_resource_parameters(
     stack_name: str,
     resource_definition: ResourceDefinition,
     resources: dict[str, ResourceDefinition],
     resource_id: str,
     func_details: FuncDetailsValue,
 ) -> dict | None:
-    params = func_details.get("parameters") or (lambda params, **kwargs: params)
+    params = func_details.get("parameters") or (
+        lambda properties, logical_resource_id, *args, **kwargs: properties
+    )
     resource_props = resource_definition["Properties"] = resource_definition.get("Properties", {})
     resource_props = dict(resource_props)
     resource_state = resource_definition.get(KEY_RESOURCE_STATE, {})
 
     if callable(params):
         # resolve parameter map via custom function
-        # TODO(srw): 1 - callable for resolving params
-        params = params(
-            resource_props,
-            stack_name=stack_name,
-            resources=resources,
-            resource_id=resource_id,
-        )
+        sig = inspect.signature(params)
+        if "logical_resource_id" in sig.parameters:
+            params = params(resource_props, resource_id, resource_definition, stack_name)
+        else:
+            raise NotImplementedError(func_details)
+            params = params(
+                resource_props,
+                stack_name=stack_name,
+                resources=resources,
+                resource_id=resource_id,
+            )
     else:
         # it could be a list like ['param1', 'param2', {'apiCallParamName': 'cfResourcePropName'}]
         if isinstance(params, list):
             _params = {}
             for param in params:
                 if isinstance(param, dict):
                     _params.update(param)
@@ -922,21 +945,30 @@
         # TODO(srw): mutably mapping params :(
         for param_key, prop_keys in dict(params).items():
             params.pop(param_key, None)
             if not isinstance(prop_keys, list):
                 prop_keys = [prop_keys]
             for prop_key in prop_keys:
                 if callable(prop_key):
-                    # TODO(srw): 2 - callable for a property value
-                    prop_value = prop_key(
-                        resource_props,
-                        stack_name=stack_name,
-                        resources=resources,
-                        resource_id=resource_id,
-                    )
+                    sig = inspect.signature(prop_key)
+                    if "logical_resource_id" in sig.parameters:
+                        prop_value = prop_key(
+                            resource_props,
+                            resource_id,
+                            resource_definition,
+                            stack_name,
+                        )
+                    else:
+                        raise NotImplementedError
+                        prop_value = prop_key(
+                            resource_props,
+                            stack_name=stack_name,
+                            resources=resources,
+                            resource_id=resource_id,
+                        )
                 else:
                     prop_value = resource_props.get(
                         prop_key,
                         resource_definition.get(prop_key, resource_state.get(prop_key)),
                     )
                 if prop_value is not None:
                     params[param_key] = prop_value
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/apigateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,16 @@
         if not role_name:
             resource["Properties"]["Name"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
-        def _api_id(params, resources, resource_id, **kwargs):
-            resource = cls(resources[resource_id])
-            return resource.physical_resource_id
+        def _api_id(properties: dict, logical_resource_id: str, resource: dict, stack_name: str):
+            return resource["PhysicalResourceId"]
 
         def _create(logical_resource_id: str, resource: dict, stack_name: str):
             client = connect_to().apigateway
             props = resource["Properties"]
 
             kwargs = select_attributes(
                 props,
@@ -284,19 +283,21 @@
             api_id, target_resource[0]["id"], resources=api_resources
         )
         result = list(filter(lambda res: res["path"] == path, api_resources))
         return result[0] if result else None
 
     @staticmethod
     def get_deploy_templates():
-        def get_apigw_resource_params(params, **kwargs):
+        def get_apigw_resource_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
             result = {
-                "restApiId": params.get("RestApiId"),
-                "pathPart": params.get("PathPart"),
-                "parentId": params.get("ParentId"),
+                "restApiId": properties.get("RestApiId"),
+                "pathPart": properties.get("PathPart"),
+                "parentId": properties.get("ParentId"),
             }
             if not result.get("parentId"):
                 # get root resource id
                 apigw = connect_to().apigateway
                 resources = apigw.get_resources(restApiId=result["restApiId"])["items"]
                 root_resource = ([r for r in resources if r["path"] == "/"] or [None])[0]
                 if not root_resource:
@@ -378,16 +379,18 @@
         """
         https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigateway-method.html
         https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-apitgateway-method-methodresponse.html
         https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-apitgateway-method-integration.html
         https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-apitgateway-method-integration-integrationresponse.html
         """
 
-        def get_params(resource_props, stack_name, resources, resource_id):
-            result = keys_to_lower(resource_props)
+        def get_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            result = keys_to_lower(properties)
             param_names = [
                 "restApiId",
                 "resourceId",
                 "httpMethod",
                 "apiKeyRequired",
                 "authorizationType",
                 "authorizerId",
@@ -496,18 +499,19 @@
         result = connect_to().apigateway.get_stage(
             restApiId=api_id, stageName=self.props["StageName"]
         )
         return result
 
     @staticmethod
     def get_deploy_templates():
-        def get_params(resource_props, stack_name, resources, resource_id):
-            stage_name = resource_props.get("StageName", "default")
-            resources[resource_id]["Properties"]["StageName"] = stage_name
-            result = keys_to_lower(resource_props)
+        def get_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            stage_name = properties.get("StageName", "default")
+            result = keys_to_lower(properties)
             param_names = [
                 "restApiId",
                 "deploymentId",
                 "description",
                 "cacheClusterEnabled",
                 "cacheClusterSize",
                 "variables",
@@ -519,14 +523,15 @@
             result = select_attributes(result, param_names)
             result["tags"] = {t["key"]: t["value"] for t in result.get("tags", [])}
             result["stageName"] = stage_name
             return result
 
         def _handle_result(result, resource_id, resources, resource_type):
             resources[resource_id]["PhysicalResourceId"] = result["stageName"]
+            resources[resource_id]["Properties"]["StageName"] = result["stageName"]
 
         return {
             "create": {
                 "function": "create_stage",
                 "parameters": get_params,
                 "result_handler": _handle_result,
             }
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/awslambda.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,21 @@
             update_config_props["Timeout"] = int(update_config_props["Timeout"])
         if "Code" in props:
             code = props["Code"] or {}
             if not code.get("ZipFile"):
                 LOG.debug(
                     'Updating code for Lambda "%s" from location: %s', props["FunctionName"], code
                 )
-            code = LambdaFunction.get_lambda_code_param(props, _include_arch=True)
+            code = LambdaFunction.get_lambda_code_param(
+                props,
+                new_resource["LogicalResourceId"],
+                new_resource,
+                stack_name,
+                _include_arch=True,
+            )
             client.update_function_code(FunctionName=props["FunctionName"], **code)
         if "Environment" in update_config_props:
             environment_variables = update_config_props["Environment"].get("Variables", {})
             update_config_props["Environment"]["Variables"] = {
                 k: str(v) for k, v in environment_variables.items()
             }
         return client.update_function_configuration(**update_config_props)
@@ -82,20 +88,28 @@
         func_name = resource.get("Properties", {}).get("FunctionName")
         if not func_name:
             resource["Properties"]["FunctionName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
-    def get_lambda_code_param(params, _include_arch=False, **kwargs):
-        code = params.get("Code", {}).copy()
+    def get_lambda_code_param(
+        properties: dict,
+        logical_resource_id: str,
+        resource: dict,
+        stack_name: str,
+        _include_arch=False,
+    ):
+        code = properties.get("Code", {}).copy()
         zip_file = code.get("ZipFile")
         if zip_file and not is_base64(zip_file) and not is_zip_file(to_bytes(zip_file)):
             tmp_dir = new_tmp_dir()
-            handler_file = get_handler_file_from_name(params["Handler"], runtime=params["Runtime"])
+            handler_file = get_handler_file_from_name(
+                properties["Handler"], runtime=properties["Runtime"]
+            )
             tmp_file = os.path.join(tmp_dir, handler_file)
             save_file(tmp_file, zip_file)
 
             # add 'cfn-response' module to archive - see:
             # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-lambda-function-code-cfnresponsemodule.html
             cloudformation_installer = cloudformation_package.get_installer()
             cloudformation_installer.install()
@@ -108,28 +122,32 @@
                 os.path.join(cfn_response_mod_dir, "index.js"),
             )
 
             # create zip file
             zip_file = create_zip_file(tmp_dir, get_content=True)
             code["ZipFile"] = zip_file
             rm_rf(tmp_dir)
-        if _include_arch and "Architectures" in params:
-            code["Architectures"] = params.get("Architectures")
+        if _include_arch and "Architectures" in properties:
+            code["Architectures"] = properties.get("Architectures")
         return code
 
     @staticmethod
     def get_deploy_templates():
-        def get_delete_params(params, **kwargs):
-            return {"FunctionName": params.get("FunctionName")}
-
-        def get_environment_params(params, **kwargs):
+        def get_delete_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            return {"FunctionName": properties.get("FunctionName")}
+
+        def get_environment_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ):
             # botocore/data/lambda/2015-03-31/service-2.json:1161 (EnvironmentVariableValue)
             # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-lambda-function-environment.html
-            if "Environment" in params:
-                environment_variables = params["Environment"].get("Variables", {})
+            if "Environment" in properties:
+                environment_variables = properties["Environment"].get("Variables", {})
                 return {"Variables": {k: str(v) for k, v in environment_variables.items()}}
 
         def result_handler(result, resource_id, resources, resource_type):
             """waits for the lambda to be in a "terminal" state, i.e. not pending"""
             resources[resource_id]["Properties"]["Arn"] = result["FunctionArn"]
             resources[resource_id]["PhysicalResourceId"] = resources[resource_id]["Properties"][
                 "FunctionName"
@@ -168,15 +186,14 @@
 
 class LambdaFunctionVersion(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Lambda::Version"
 
     def fetch_state(self, stack_name, resources):
-
         props = self.props
         if not self.physical_resource_id:
             return None
 
         function_name = props["FunctionName"]
         qualifier = props["Version"]
 
@@ -283,34 +300,36 @@
 
     @staticmethod
     def get_deploy_templates():
         def _store_physical_id(result, resource_id, resources, resource_type):
             parsed_statement = json.loads(result["Statement"])
             resources[resource_id]["PhysicalResourceId"] = parsed_statement["Sid"]
 
-        def lambda_permission_params(params, resources, resource_id, **kwargs):
+        def lambda_permission_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
             result = select_parameters("FunctionName", "Action", "Principal", "SourceArn")(
-                params, **kwargs
+                properties, logical_resource_id, resource, stack_name
             )
             # generate SID
             # e.g. stack-78d0ac66-fnAllowInvokeLambdaPermissionsStacktopicF723B1A748672DB5-1D7VMEAZ2UQIN
             # e.g. stack-6283277e-fnAllowInvokeLambdaPermissionsStacktopicF48672DB5-19EAQW5GIWOS5 when the functional ID is shorter
             suffix = "".join(random.choices(string.digits + string.ascii_uppercase, k=13))
-            prefix = kwargs.get("stack_name")
+            prefix = stack_name
             if prefix:
-                result["StatementId"] = f"{prefix}-{resource_id}-{suffix}"
+                result["StatementId"] = f"{prefix}-{logical_resource_id}-{suffix}"
             else:
-                result["StatementId"] = f"{resource_id}-{suffix}"
+                result["StatementId"] = f"{logical_resource_id}-{suffix}"
             return result
 
-        def get_delete_params(params, **kwargs):
-            resources = kwargs["resources"]
-            resource_id = kwargs["resource_id"]
-            statement_id = resources[resource_id]["PhysicalResourceId"]
-            return {"FunctionName": params.get("FunctionName"), "StatementId": statement_id}
+        def get_delete_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            statement_id = resource["PhysicalResourceId"]
+            return {"FunctionName": properties.get("FunctionName"), "StatementId": statement_id}
 
         return {
             "create": {
                 "function": "add_permission",
                 "parameters": lambda_permission_params,
                 "result_handler": _store_physical_id,
             },
@@ -518,17 +537,19 @@
         parts = layer_arn.split(":")
         layer_name = parts[6] if ":" in layer_arn else layer_arn
         version_number = int(parts[7] if len(parts) > 7 else 1)  # TODO fetch latest version number
         return layer_name, version_number
 
     @classmethod
     def get_deploy_templates(cls):
-        def layer_permission_params(params, **kwargs):
-            layer_name, version_number = cls.layer_name_and_version(params)
-            result = select_attributes(params, ["Action", "Principal"])
+        def layer_permission_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ):
+            layer_name, version_number = cls.layer_name_and_version(properties)
+            result = select_attributes(properties, ["Action", "Principal"])
             result["StatementId"] = short_uid()
             result["LayerName"] = layer_name
             result["VersionNumber"] = version_number
             return result
 
         return {
             "create": {
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,19 @@
         result = client.list_certificates().get("CertificateSummaryList", [])
         domain_name = self.props.get("DomainName")
         result = [c for c in result if c["DomainName"] == domain_name]
         return (result or [None])[0]
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create_params(params, *args, **kwargs):
+        def _create_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
             result = select_attributes(
-                params,
+                properties,
                 [
                     "CertificateAuthorityArn",
                     "DomainName",
                     "DomainValidationOptions",
                     "SubjectAlternativeNames",
                     "Tags",
                     "ValidationMethod",
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/cloudformation.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,28 +48,30 @@
         if not role_name:
             resource["Properties"]["StackName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
-        def get_nested_stack_params(params, **kwargs):
-            nested_stack_name = params["StackName"]
-            stack_params = params.get("Parameters", {})
-            stack_params = [
+        def get_nested_stack_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ):
+            nested_stack_name = properties["StackName"]
+            stack_parameters = properties.get("Parameters", {})
+            stack_parameters = [
                 {
                     "ParameterKey": k,
                     "ParameterValue": str(v).lower() if isinstance(v, bool) else str(v),
                 }
-                for k, v in stack_params.items()
+                for k, v in stack_parameters.items()
             ]
             result = {
                 "StackName": nested_stack_name,
-                "TemplateURL": params.get("TemplateURL"),
-                "Parameters": stack_params,
+                "TemplateURL": properties.get("TemplateURL"),
+                "Parameters": stack_parameters,
             }
             return result
 
         def result_handler(result, resource_id: str, resources: dict, resource_type: str):
             resource = resources[resource_id]
             resource["PhysicalResourceId"] = result["StackId"]
             connect_to().cloudformation.get_waiter("stack_create_complete").wait(
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,18 @@
 
     @classmethod
     def get_deploy_templates(cls):
         def _handle_result(result, resource_id, resources, resource_type):
             resource = resources[resource_id]
             resources[resource_id]["PhysicalResourceId"] = resource["Properties"]["AlarmName"]
 
-        def get_delete_params(params, **kwargs):
-            return {"AlarmNames": [params["AlarmName"]]}
+        def get_delete_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            return {"AlarmNames": [properties["AlarmName"]]}
 
         return {
             "create": {"function": cls._create_function_name(), "result_handler": _handle_result},
             "delete": {"function": "delete_alarms", "parameters": get_delete_params},
         }
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/dynamodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,22 @@
     generate_default_name,
 )
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.utils import common
 from localstack.utils.aws import aws_stack
 
 
-def get_ddb_provisioned_throughput(params, **kwargs):
+def get_ddb_provisioned_throughput(
+    properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+) -> dict | None:
     # see https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-dynamodb-table.html#cfn-dynamodb-table-provisionedthroughput
-    args = params.get("ProvisionedThroughput")
+    args = properties.get("ProvisionedThroughput")
     if args == PLACEHOLDER_AWS_NO_VALUE:
         return None
-    is_ondemand = params.get("BillingMode") == "PAY_PER_REQUEST"
+    is_ondemand = properties.get("BillingMode") == "PAY_PER_REQUEST"
     # if the BillingMode is set to PAY_PER_REQUEST, you cannot specify ProvisionedThroughput
     # if the BillingMode is set to PROVISIONED (default), you have to specify ProvisionedThroughput
 
     if args is None:
         if is_ondemand:
             # do not return default value if it's on demand
             return
@@ -31,17 +33,19 @@
         args["ReadCapacityUnits"] = int(args["ReadCapacityUnits"])
     if isinstance(args["WriteCapacityUnits"], str):
         args["WriteCapacityUnits"] = int(args["WriteCapacityUnits"])
 
     return args
 
 
-def get_ddb_global_sec_indexes(params: dict, **kwargs) -> list | None:
-    args: list = params.get("GlobalSecondaryIndexes")
-    is_ondemand = params.get("BillingMode") == "PAY_PER_REQUEST"
+def get_ddb_global_sec_indexes(
+    properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+) -> list | None:
+    args: list = properties.get("GlobalSecondaryIndexes")
+    is_ondemand = properties.get("BillingMode") == "PAY_PER_REQUEST"
     if not args:
         return
 
     for index in args:
         # we ignore ContributorInsightsSpecification as not supported yet in DynamoDB and CloudWatch
         index.pop("ContributorInsightsSpecification", None)
         provisioned_throughput = index.get("ProvisionedThroughput")
@@ -54,18 +58,20 @@
             if isinstance((write_units := provisioned_throughput["WriteCapacityUnits"]), str):
                 provisioned_throughput["WriteCapacityUnits"] = int(write_units)
         else:
             raise Exception("Can't specify ProvisionedThroughput with PAY_PER_REQUEST")
     return args
 
 
-def get_ddb_kinesis_stream_specification(params, **kwargs):
-    args = params.get("KinesisStreamSpecification")
+def get_ddb_kinesis_stream_specification(
+    properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+) -> dict:
+    args = properties.get("KinesisStreamSpecification")
     if args:
-        args["TableName"] = params["TableName"]
+        args["TableName"] = properties["TableName"]
     return args
 
 
 class DynamoDBTable(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::DynamoDB::Table"
@@ -105,17 +111,17 @@
                         "TableName": "TableName",
                         "AttributeDefinitions": "AttributeDefinitions",
                         "KeySchema": "KeySchema",
                         "BillingMode": "BillingMode",
                         "ProvisionedThroughput": get_ddb_provisioned_throughput,
                         "LocalSecondaryIndexes": "LocalSecondaryIndexes",
                         "GlobalSecondaryIndexes": get_ddb_global_sec_indexes,
-                        "StreamSpecification": lambda params, **kwargs: (
+                        "StreamSpecification": lambda properties, logical_resource_id, *args, **kwargs: (
                             common.merge_dicts(
-                                params.get("StreamSpecification"),
+                                properties.get("StreamSpecification"),
                                 {"StreamEnabled": True},
                                 default=None,
                             )
                         ),
                     },
                     "result_handler": _set_attributes,
                 },
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import remove_none_values
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.utils.aws import arns, aws_stack
 from localstack.utils.collections import convert_to_typed_dict
 
 
-def es_add_tags_params(params, **kwargs):
-    es_arn = arns.es_domain_arn(params.get("DomainName"))
-    tags = params.get("Tags", [])
+def es_add_tags_params(properties: dict, logical_resource_id: str, resource: dict, stack_name: str):
+    es_arn = arns.es_domain_arn(properties.get("DomainName"))
+    tags = properties.get("Tags", [])
     return {"ARN": es_arn, "TagList": tags}
 
 
 class ElasticsearchDomain(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Elasticsearch::Domain"
@@ -35,16 +35,18 @@
         )
 
     def _domain_name(self):
         return self.props.get("DomainName") or self.logical_resource_id
 
     @staticmethod
     def get_deploy_templates():
-        def _create_params(params, **kwargs):
-            result = convert_to_typed_dict(CreateElasticsearchDomainRequest, params)
+        def _create_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ):
+            result = convert_to_typed_dict(CreateElasticsearchDomainRequest, properties)
             result = remove_none_values(result)
             cluster_config = result.get("ElasticsearchClusterConfig")
             if isinstance(cluster_config, dict):
                 # set defaults required for boto3 calls
                 cluster_config.setdefault("DedicatedMasterType", "m3.medium.elasticsearch")
                 cluster_config.setdefault("WarmType", "ultrawarm1.medium.elasticsearch")
             return result
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,24 +101,28 @@
         if not role_name:
             resource["Properties"]["Name"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
-        def events_put_rule_params(params, **kwargs):
+        def events_put_rule_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
             attrs = [
                 "ScheduleExpression",
                 "EventPattern",
                 "State",
                 "Description",
                 "Name",
                 "EventBusName",
             ]
-            result = select_parameters(*attrs)(params, **kwargs)
+            result = select_parameters(*attrs)(
+                properties, logical_resource_id, resource, stack_name
+            )
 
             # TODO: remove this when refactoring events (prefix etc. was excluded here already to avoid most of the wrong behavior)
             def wrap_in_lists(o, **kwargs):
                 if isinstance(o, dict):
                     for k, v in o.items():
                         if not isinstance(v, (dict, list)) and k not in [
                             "prefix",
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,34 +274,36 @@
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def _post_create(cls, logical_resource_id: str, resource: dict, stack_name: str):
         """attaches managed policies from the template to the role"""
 
+        properties = resource["Properties"]
         iam = aws_stack.connect_to_service("iam")
-        props = resource["Properties"]
-        role_name = props["RoleName"]
+        role_name = properties["RoleName"]
 
         # attach managed policies
-        policy_arns = props.get("ManagedPolicyArns", [])
+        policy_arns = properties.get("ManagedPolicyArns", [])
         for arn in policy_arns:
             iam.attach_role_policy(RoleName=role_name, PolicyArn=arn)
 
         # add inline policies
-        inline_policies = props.get("Policies", [])
+        inline_policies = properties.get("Policies", [])
         for policy in inline_policies:
             assert not isinstance(
                 policy, list
             )  # remove if this doesn't make any problems for a while
             if policy == PLACEHOLDER_AWS_NO_VALUE:
                 continue
             if not isinstance(policy, dict):
                 LOG.info(
-                    'Invalid format of policy for IAM role "%s": %s', props.get("RoleName"), policy
+                    'Invalid format of policy for IAM role "%s": %s',
+                    properties.get("RoleName"),
+                    policy,
                 )
                 continue
             pol_name = policy.get("PolicyName")
 
             # get policy document - make sure we're resolving references in the policy doc
             doc = dict(policy["PolicyDocument"])
             doc = remove_none_values(doc)
@@ -310,15 +312,15 @@
             statements = ensure_list(doc["Statement"])
             for statement in statements:
                 if isinstance(statement.get("Resource"), list):
                     # filter out empty resource strings
                     statement["Resource"] = [r for r in statement["Resource"] if r]
             doc = json.dumps(doc)
             iam.put_role_policy(
-                RoleName=props["RoleName"],
+                RoleName=properties["RoleName"],
                 PolicyName=pol_name,
                 PolicyDocument=doc,
             )
 
     @staticmethod
     def _pre_delete(logical_resource_id: str, resource: dict, stack_name: str):
         """detach managed policies from role before deleting"""
@@ -480,16 +482,18 @@
                     UserName=user, PolicyName=policy_name, PolicyDocument=policy_doc
                 )
             for group in props.get("Groups", []):
                 iam.put_group_policy(
                     GroupName=group, PolicyName=policy_name, PolicyDocument=policy_doc
                 )
 
-        def _delete_params(params, *args, **kwargs):
-            return {"PolicyArn": arns.policy_arn(params["PolicyName"])}
+        def _delete_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            return {"PolicyArn": arns.policy_arn(properties["PolicyName"])}
 
         return {
             "create": {
                 "function": _create,
                 "result_handler": _store_physical_id,
             },
             "delete": {"function": "delete_policy", "parameters": _delete_params},
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/kinesis.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,18 @@
 
         shard_count = props.get("ShardCount")
         if shard_count is None:
             props["ShardCount"] = 1
 
     @staticmethod
     def get_deploy_templates():
-        def get_delete_params(params, **kwargs):
-            return {"StreamName": params["Name"], "EnforceConsumerDeletion": True}
+        def get_delete_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            return {"StreamName": properties["Name"], "EnforceConsumerDeletion": True}
 
         def _store_arn(result, resource_id, resources, resource_type):
             client = aws_stack.connect_to_service("kinesis")
             stream_name = resources[resource_id]["Properties"]["Name"]
 
             description = client.describe_stream(StreamName=stream_name)
             while description["StreamDescription"]["StreamStatus"] != "ACTIVE":
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/opensearch.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 from localstack.utils.aws import arns, aws_stack
 from localstack.utils.collections import convert_to_typed_dict
 
 
 # OpenSearch still uses "es" ARNs
 # See examples in:
 # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-opensearchservice-domain.html
-def opensearch_add_tags_params(params, **kwargs):
-    es_arn = arns.es_domain_arn(params.get("DomainName"))
-    tags = params.get("Tags", [])
+def opensearch_add_tags_params(
+    properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+):
+    es_arn = arns.es_domain_arn(properties.get("DomainName"))
+    tags = properties.get("Tags", [])
     return {"ARN": es_arn, "TagList": tags}
 
 
 class OpenSearchDomain(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::OpenSearchService::Domain"
@@ -28,17 +30,19 @@
         return aws_stack.connect_to_service("opensearch").describe_domain(DomainName=domain_name)
 
     def _domain_name(self):
         return self.props.get("DomainName") or self.logical_resource_id
 
     @staticmethod
     def get_deploy_templates():
-        def _create_params(params, **kwargs):
-            params = remove_none_values(params)
-            result = convert_to_typed_dict(CreateDomainRequest, params)
+        def _create_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ):
+            properties = remove_none_values(properties)
+            result = convert_to_typed_dict(CreateDomainRequest, properties)
             cluster_config = result.get("ClusterConfig")
             if isinstance(cluster_config, dict):
                 # set defaults required for boto3 calls
                 cluster_config.setdefault(
                     "DedicatedMasterType", OpenSearchPartitionInstanceType.m3_medium_search
                 )
                 cluster_config.setdefault(
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/route53.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,48 +15,52 @@
             "ResourceRecordSets"
         ]
         result = [r for r in result if r["Name"] == props["Name"] and r["Type"] == props["Type"]]
         return (result or [None])[0]
 
     @staticmethod
     def get_deploy_templates():
-        def param_change_batch(params, **kwargs):
+        def param_change_batch(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ):
             attr_names = [
                 "Name",
                 "Type",
                 "SetIdentifier",
                 "Weight",
                 "Region",
                 "GeoLocation",
                 "Failover",
                 "MultiValueAnswer",
                 "TTL",
                 "ResourceRecords",
                 "AliasTarget",
                 "HealthCheckId",
             ]
-            attrs = select_attributes(params, attr_names)
+            attrs = select_attributes(properties, attr_names)
             if "TTL" in attrs:
                 if isinstance(attrs["TTL"], str):
                     attrs["TTL"] = int(attrs["TTL"])
 
             alias_target = attrs.get("AliasTarget", {})
             alias_target["EvaluateTargetHealth"] = alias_target.get("EvaluateTargetHealth", False)
             if "ResourceRecords" in attrs:
                 attrs["ResourceRecords"] = [{"Value": r} for r in attrs["ResourceRecords"]]
             return {
-                "Comment": params.get("Comment", ""),
+                "Comment": properties.get("Comment", ""),
                 "Changes": [{"Action": "CREATE", "ResourceRecordSet": attrs}],
             }
 
-        def hosted_zone_id_change_batch(params, **kwargs):
+        def hosted_zone_id_change_batch(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ):
             route53 = aws_stack.connect_to_service("route53")
-            hosted_zone_id = params.get("HostedZoneId")
+            hosted_zone_id = properties.get("HostedZoneId")
             if not hosted_zone_id:
-                hosted_zone_name = params.get("HostedZoneName")
+                hosted_zone_name = properties.get("HostedZoneName")
                 # https://docs.aws.amazon.com/Route53/latest/APIReference/API_ChangeResourceRecordSets.html"
                 # "Specify either HostedZoneName or HostedZoneId, but not both. If you have multiple hosted zones with
                 # the same domain name, you must specify the hosted zone using HostedZoneId."
                 if not hosted_zone_name:
                     raise Exception("Either HostedZoneId or HostedZoneName must be present.")
                 hosted_zones = route53.list_hosted_zones_by_name(DNSName=hosted_zone_name)[
                     "HostedZones"
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,16 +119,18 @@
                 if (allowed_headers := cfn_rule.get("Id")) is not None:
                     rule["ID"] = allowed_headers
 
                 cors_rules.append(rule)
 
             return {"CORSRules": cors_rules}
 
-        def s3_bucket_notification_config(params, **kwargs):
-            notif_config = params.get("NotificationConfiguration")
+        def s3_bucket_notification_config(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict | None:
+            notif_config = properties.get("NotificationConfiguration")
             if not notif_config:
                 return None
 
             lambda_configs = []
             queue_configs = []
             topic_configs = []
 
@@ -153,15 +155,15 @@
                     }
                     if filter_rules:
                         entry["Filter"] = {"Key": {"FilterRules": filter_rules}}
                     attrs[1].append(entry)
 
             # construct final result
             result = {
-                "Bucket": params.get("BucketName"),
+                "Bucket": properties.get("BucketName"),
                 "NotificationConfiguration": {
                     "LambdaFunctionConfigurations": lambda_configs,
                     "QueueConfigurations": queue_configs,
                     "TopicConfigurations": topic_configs,
                 },
             }
             return result
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,18 +73,20 @@
         if not name:
             resource["Properties"]["Name"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create_params(params, **kwargs):
+        def _create_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
             attributes = ["Name", "Description", "KmsKeyId", "SecretString", "Tags"]
-            result = select_attributes(params, attributes)
-            gen_secret = params.get("GenerateSecretString")
+            result = select_attributes(properties, attributes)
+            gen_secret = properties.get("GenerateSecretString")
             if gen_secret:
                 excl_lower = gen_secret.get("ExcludeLowercase")
                 excl_upper = gen_secret.get("ExcludeUppercase")
                 excl_chars = gen_secret.get("ExcludeCharacters") or ""
                 excl_numbers = gen_secret.get("ExcludeNumbers")
                 excl_punct = gen_secret.get("ExcludePunctuation")
                 incl_spaces = gen_secret.get("IncludeSpace")
@@ -154,19 +156,21 @@
         result = aws_stack.connect_to_service("secretsmanager").get_resource_policy(
             SecretId=secret_id
         )
         return result
 
     @staticmethod
     def get_deploy_templates():
-        def create_params(params, **kwargs):
+        def create_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
             return {
-                "SecretId": params["SecretId"].split(":")[-1],
-                "ResourcePolicy": json.dumps(params["ResourcePolicy"]),
-                "BlockPublicPolicy": params.get("BlockPublicPolicy"),
+                "SecretId": properties["SecretId"].split(":")[-1],
+                "ResourcePolicy": json.dumps(properties["ResourcePolicy"]),
+                "BlockPublicPolicy": properties.get("BlockPublicPolicy"),
             }
 
         def _set_physical_resource_id(
             result: dict, resource_id: str, resources: dict, resource_type: str
         ):
             resource = resources[resource_id]
             resource["PhysicalResourceId"] = arns.secretsmanager_secret_arn(
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/sns.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,36 +33,40 @@
         if not role_name:
             resource["Properties"]["TopicName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
-        def _create_params(params, *args, **kwargs):
+        def _create_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
             attributes = {}
-            dedup = params.get("ContentBasedDeduplication")
-            display_name = params.get("DisplayName")
-            fifo_topic = params.get("FifoTopic")
-            kms_master_key = params.get("KmsMasterKeyId")
-            tags = params.get("Tags") or []
-            topic_name = params.get("TopicName")
+            dedup = properties.get("ContentBasedDeduplication")
+            display_name = properties.get("DisplayName")
+            fifo_topic = properties.get("FifoTopic")
+            kms_master_key = properties.get("KmsMasterKeyId")
+            tags = properties.get("Tags") or []
+            topic_name = properties.get("TopicName")
             if dedup is not None:
                 attributes["ContentBasedDeduplication"] = canonicalize_bool_to_str(dedup)
             if display_name:
                 attributes["DisplayName"] = display_name
             if fifo_topic is not None:
                 attributes["FifoTopic"] = canonicalize_bool_to_str(fifo_topic)
             if kms_master_key:
                 attributes["KmsMasterKeyId"] = kms_master_key
             result = {"Name": topic_name, "Attributes": attributes, "Tags": tags}
             return result
 
-        def _topic_arn(params, resources, resource_id, **kwargs):
-            resource = cls(resources[resource_id])
-            return resource.physical_resource_id
+        def _topic_arn(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            provider = cls(resource)
+            return provider.physical_resource_id
 
         def _list_all_topics(sns_client):
             rs = sns_client.list_topics()
             topics = rs.get("Topics", [])
             key = rs.get("NextToken")
 
             while key and key != "":
@@ -127,29 +131,32 @@
             if props.get("Protocol") == sub["Protocol"] and props.get("Endpoint") == sub["Endpoint"]
         ]
         # TODO: use get_subscription_attributes to compare FilterPolicy
         return result[0] if result else None
 
     @staticmethod
     def get_deploy_templates():
-        def sns_subscription_arn(params, resources, resource_id, **kwargs):
-            resource = resources[resource_id]
+        def sns_subscription_arn(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
             return resource["PhysicalResourceId"]
 
-        def sns_subscription_params(params, **kwargs):
+        def sns_subscription_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
             def attr_val(val):
                 return json.dumps(val) if isinstance(val, (dict, list)) else str(val)
 
             attrs = [
                 "DeliveryPolicy",
                 "FilterPolicy",
                 "RawMessageDelivery",
                 "RedrivePolicy",
             ]
-            result = {a: attr_val(params[a]) for a in attrs if a in params}
+            result = {a: attr_val(properties[a]) for a in attrs if a in properties}
             return result
 
         def _set_physical_resource_id(
             result: dict, resource_id: str, resources: dict, resource_type: str
         ):
             resources[resource_id]["PhysicalResourceId"] = result["SubscriptionArn"]
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/sqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,21 +100,20 @@
                 stack_name, resource["LogicalResourceId"]
             )
             if resource["Properties"].get("FifoQueue"):
                 resource["Properties"]["QueueName"] += ".fifo"
 
     @classmethod
     def get_deploy_templates(cls):
-        def _queue_url(params, resources, resource_id, **kwargs):
-            resource = cls(resources[resource_id])
-            props = resource.props
-            queue_url = resource.physical_resource_id or props.get("QueueUrl")
+        def _queue_url(properties: dict, logical_resource_id: str, resource: dict, stack_name: str):
+            provider = cls(resource)
+            queue_url = provider.physical_resource_id or properties.get("QueueUrl")
             if queue_url:
                 return queue_url
-            return arns.sqs_queue_url_for_arn(props["QueueArn"])
+            return arns.sqs_queue_url_for_arn(properties["QueueArn"])
 
         def _set_physical_resource_id(
             result: dict, resource_id: str, resources: dict, resource_type: str
         ):
             resources[resource_id]["PhysicalResourceId"] = result["QueueUrl"]
 
         return {
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,37 +87,39 @@
 
     @classmethod
     def get_deploy_templates(cls):
         def result_handler(result, resource_id, resources, resource_type):
             resources[resource_id]["Properties"]["Arn"] = result["stateMachineArn"]
             resources[resource_id]["PhysicalResourceId"] = result["stateMachineArn"]
 
-        def _create_params(params, **kwargs):
-            def _get_definition(params):
+        def _create_params(
+            properties: dict, logical_resource_id: str, resource: dict, stack_name: str
+        ) -> dict:
+            def _get_definition(properties):
                 # TODO: support "Definition" parameter
-                definition_str = params.get("DefinitionString")
-                s3_location = params.get("DefinitionS3Location")
+                definition_str = properties.get("DefinitionString")
+                s3_location = properties.get("DefinitionS3Location")
                 if not definition_str and s3_location:
                     # TODO: currently not covered by tests - add a test to mimick the behavior of "sam deploy ..."
                     s3_client = aws_stack.connect_to_service("s3")
                     LOG.debug("Fetching state machine definition from S3: %s", s3_location)
                     result = s3_client.get_object(
                         Bucket=s3_location["Bucket"], Key=s3_location["Key"]
                     )
                     definition_str = to_str(result["Body"].read())
-                substitutions = params.get("DefinitionSubstitutions")
+                substitutions = properties.get("DefinitionSubstitutions")
                 if substitutions is not None:
                     definition_str = _apply_substitutions(definition_str, substitutions)
                 return definition_str
 
             return {
-                "name": params.get("StateMachineName"),
-                "definition": _get_definition(params),
-                "roleArn": params.get("RoleArn"),
-                "type": params.get("StateMachineType", None),
+                "name": properties.get("StateMachineName"),
+                "definition": _get_definition(properties),
+                "roleArn": properties.get("RoleArn"),
+                "type": properties.get("StateMachineType", None),
             }
 
         return {
             "create": {
                 "function": "create_state_machine",
                 "parameters": _create_params,
                 "result_handler": result_handler,
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230620171514/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/state/core.py` & `localstack-core-2.1.1.dev20230620171514/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230620171514/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230620171514/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230620171514/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230620171514/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/collections.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230620171514/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230619173831
+Version: 2.1.1.dev20230620171514
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8628787878787878%*

 * *Differences: {"'localstack.hooks.on_infra_shutdown'": '{insert: [(1, '*

 * *                                         "'_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown')], "*

 * *                                         'delete: [0]}',*

 * * "'localstack.hooks.on_infra_start'": '{insert: [(2, '*

 * *                                      "'deprecation_warnings=localstack.plugins:deprecation_warnings'), "*

 * *                                      '(3, '*

 * *                                      "'register_partition […]*

```diff
@@ -49,40 +49,40 @@
         "configure_edge_port=localstack.plugins:configure_edge_port"
     ],
     "localstack.hooks.on_infra_ready": [
         "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
         "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
-        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
+        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
     ],
     "localstack.hooks.on_infra_start": [
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
-        "deprecation_warnings=localstack.plugins:deprecation_warnings",
-        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser"
+        "deprecation_warnings=localstack.plugins:deprecation_warnings",
+        "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration"
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
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
         "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
         "terraform/community=localstack.packages.plugins:terraform_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
         "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package"
+        "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
+        "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
+        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230619173831/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230620171514/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/pyproject.toml` & `localstack-core-2.1.1.dev20230620171514/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230619173831/setup.cfg` & `localstack-core-2.1.1.dev20230620171514/setup.cfg`

 * *Files identical despite different names*

