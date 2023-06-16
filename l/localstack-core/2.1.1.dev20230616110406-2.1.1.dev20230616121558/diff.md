# Comparing `tmp/localstack-core-2.1.1.dev20230616110406.tar.gz` & `tmp/localstack-core-2.1.1.dev20230616121558.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230616110406.tar", last modified: Fri Jun 16 11:04:13 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230616121558.tar", last modified: Fri Jun 16 12:16:05 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230616110406.tar` & `localstack-core-2.1.1.dev20230616121558.tar`

### file list

```diff
@@ -1,851 +1,852 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.233463 localstack-core-2.1.1.dev20230616110406/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-16 11:04:13.233463 localstack-core-2.1.1.dev20230616110406/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.137461 localstack-core-2.1.1.dev20230616110406/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.137461 localstack-core-2.1.1.dev20230616110406/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-16 11:04:06.000000 localstack-core-2.1.1.dev20230616110406/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.137461 localstack-core-2.1.1.dev20230616110406/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.137461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.137461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.137461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.137461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   755634 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.141461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.145461 localstack-core-2.1.1.dev20230616110406/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.149461 localstack-core-2.1.1.dev20230616110406/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.149461 localstack-core-2.1.1.dev20230616110406/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.149461 localstack-core-2.1.1.dev20230616110406/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.149461 localstack-core-2.1.1.dev20230616110406/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.149461 localstack-core-2.1.1.dev20230616110406/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.149461 localstack-core-2.1.1.dev20230616110406/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.153461 localstack-core-2.1.1.dev20230616110406/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.153461 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    61609 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14059 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.153461 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.161462 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.165462 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.165462 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.165462 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.165462 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65108 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.169462 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33005 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20991 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7434 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2190 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21924 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2949 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3188 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9196 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28213 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3327 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4787 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2640 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13639 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6708 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8678 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5134 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3927 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5754 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5500 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.169462 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.169462 localstack-core-2.1.1.dev20230616110406/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.169462 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.169462 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.169462 localstack-core-2.1.1.dev20230616110406/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.169462 localstack-core-2.1.1.dev20230616110406/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.169462 localstack-core-2.1.1.dev20230616110406/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35960 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52790 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.173462 localstack-core-2.1.1.dev20230616110406/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.177462 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.177462 localstack-core-2.1.1.dev20230616110406/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.177462 localstack-core-2.1.1.dev20230616110406/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.177462 localstack-core-2.1.1.dev20230616110406/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.177462 localstack-core-2.1.1.dev20230616110406/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43901 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.177462 localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.177462 localstack-core-2.1.1.dev20230616110406/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.181462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.181462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.181462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.181462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.181462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.181462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.181462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.185462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.185462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.185462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.185462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.185462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.189462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.189462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.189462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.193462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.193462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.193462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.193462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.197462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.197462 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.201463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.205463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.209463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.209463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.209463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.209463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.209463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.209463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.213463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.213463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.217463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.221463 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.221463 localstack-core-2.1.1.dev20230616110406/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.221463 localstack-core-2.1.1.dev20230616110406/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.221463 localstack-core-2.1.1.dev20230616110406/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.221463 localstack-core-2.1.1.dev20230616110406/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.221463 localstack-core-2.1.1.dev20230616110406/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.221463 localstack-core-2.1.1.dev20230616110406/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.225463 localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.225463 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69752 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.225463 localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.229463 localstack-core-2.1.1.dev20230616110406/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.229463 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.229463 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.229463 localstack-core-2.1.1.dev20230616110406/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.229463 localstack-core-2.1.1.dev20230616110406/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.233463 localstack-core-2.1.1.dev20230616110406/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.233463 localstack-core-2.1.1.dev20230616110406/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:04:13.233463 localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-16 11:04:13.000000 localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37808 2023-06-16 11:04:13.000000 localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 11:04:13.000000 localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-16 11:04:13.000000 localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 11:04:09.000000 localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-16 11:04:09.000000 localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-16 11:04:13.000000 localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-16 11:04:13.000000 localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-16 11:04:13.233463 localstack-core-2.1.1.dev20230616110406/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-16 10:32:52.000000 localstack-core-2.1.1.dev20230616110406/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.609835 localstack-core-2.1.1.dev20230616121558/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-16 12:16:05.609835 localstack-core-2.1.1.dev20230616121558/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.521837 localstack-core-2.1.1.dev20230616121558/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.521837 localstack-core-2.1.1.dev20230616121558/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-16 12:15:58.000000 localstack-core-2.1.1.dev20230616121558/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.521837 localstack-core-2.1.1.dev20230616121558/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   755634 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61609 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14059 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65108 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33005 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20991 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7434 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2190 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21924 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2949 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3188 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9196 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28213 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3327 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4787 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2640 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13639 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6708 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8678 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5134 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3927 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5754 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5500 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59474 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43901 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.585836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.585836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.585836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.601835 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69752 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.601835 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.601835 localstack-core-2.1.1.dev20230616121558/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.609835 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37846 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 12:16:02.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-16 12:16:02.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-16 12:16:05.609835 localstack-core-2.1.1.dev20230616121558/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230616110406/LICENSE.txt` & `localstack-core-2.1.1.dev20230616121558/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/Makefile` & `localstack-core-2.1.1.dev20230616121558/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/PKG-INFO` & `localstack-core-2.1.1.dev20230616121558/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230616110406
+Version: 2.1.1.dev20230616121558
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230616110406/README.md` & `localstack-core-2.1.1.dev20230616121558/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/bin/localstack` & `localstack-core-2.1.1.dev20230616121558/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230616121558/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230616121558/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230616121558/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230616121558/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230616121558/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230616121558/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230616121558/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/config.py` & `localstack-core-2.1.1.dev20230616121558/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/constants.py` & `localstack-core-2.1.1.dev20230616121558/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230616121558/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/client.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/request.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/response.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/http/router.py` & `localstack-core-2.1.1.dev20230616121558/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230616121558/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230616121558/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230616121558/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230616121558/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230616121558/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230616121558/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/packages/ffmpeg.py` & `localstack-core-2.1.1.dev20230616121558/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230616121558/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/plugins.py` & `localstack-core-2.1.1.dev20230616121558/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230616121558/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230616121558/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230616121558/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230616121558/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230616121558/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,41 +9,40 @@
 import struct
 import uuid
 from collections import namedtuple
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Tuple
 
 from cryptography.exceptions import InvalidSignature
+from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, hmac
 from cryptography.hazmat.primitives import serialization as crypto_serialization
 from cryptography.hazmat.primitives.asymmetric import ec, padding, rsa, utils
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
 
 from localstack.aws.accounts import get_aws_account_id
-from localstack.aws.api import CommonServiceException
 from localstack.aws.api.kms import (
     CreateAliasRequest,
     CreateGrantRequest,
     CreateKeyRequest,
-    DisabledException,
     EncryptionContextType,
     KeyMetadata,
     KeyState,
     KMSInvalidMacException,
     KMSInvalidSignatureException,
-    KMSInvalidStateException,
     MacAlgorithmSpec,
     MessageType,
-    NotFoundException,
     OriginType,
     SigningAlgorithmSpec,
     UnsupportedOperationException,
 )
+from localstack.services.kms.exceptions import ValidationException
 from localstack.services.kms.utils import is_valid_key_arn
 from localstack.services.stores import AccountRegionBundle, BaseStore, LocalAttribute
-from localstack.utils.aws.arns import kms_alias_arn, kms_key_arn, parse_arn
+from localstack.utils.aws.arns import kms_alias_arn, kms_key_arn
 from localstack.utils.crypto import decrypt, encrypt
 from localstack.utils.strings import long_uid, to_bytes, to_str
 
 LOG = logging.getLogger(__name__)
 
 PATTERN_UUID = re.compile(
     r"^[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}$"
@@ -68,25 +67,14 @@
 HMAC_RANGE_KEY_LENGTHS = {
     "HMAC_224": (28, 64),
     "HMAC_256": (32, 64),
     "HMAC_384": (48, 128),
     "HMAC_512": (64, 128),
 }
 
-
-class ValidationException(CommonServiceException):
-    def __init__(self, message: str):
-        super().__init__("ValidationException", message, 400, True)
-
-
-class AccessDeniedException(CommonServiceException):
-    def __init__(self, message: str):
-        super().__init__("AccessDeniedException", message, 400, True)
-
-
 KEY_ID_LEN = 36
 # Moto uses IV_LEN of 12, as it is fine for GCM encryption mode, but we use CBC, so have to set it to 16.
 IV_LEN = 16
 TAG_LEN = 16
 CIPHERTEXT_HEADER_FORMAT = ">{key_id_len}s{iv_len}s{tag_len}s".format(
     key_id_len=KEY_ID_LEN, iv_len=IV_LEN, tag_len=TAG_LEN
 )
@@ -162,32 +150,36 @@
     1. Keys that are created to be used inside of AWS. For such a key, its key material / private key are not to
     leave AWS unencrypted. If they have to leave AWS, a different KmsCryptoKey is used to encrypt the data first.
     2. Keys that AWS creates for customers for some external use. Such a key might be returned to a customer with its
     key material or public key unencrypted - see KMS GenerateDataKey / GenerateDataKeyPair. But such a key is not stored
     by AWS and is not used by AWS.
     """
 
+    public_key: Optional[bytes]
+    private_key: Optional[bytes]
+    key_material: bytes
+
     def __init__(self, key_spec: str):
         self.private_key = None
         self.public_key = None
         # Technically, key_material, being a symmetric encryption key, is only relevant for
         #   key_spec == SYMMETRIC_DEFAULT.
         # But LocalStack uses symmetric encryption with this key_material even for other specs. Asymmetric keys are
         # generated, but are not actually used.
         self.key_material = os.urandom(SYMMETRIC_DEFAULT_MATERIAL_LENGTH)
 
         if key_spec == "SYMMETRIC_DEFAULT":
             return
 
         if key_spec.startswith("RSA"):
             key_size = RSA_CRYPTO_KEY_LENGTHS.get(key_spec)
-            self.key = rsa.generate_private_key(public_exponent=65537, key_size=key_size)
+            key = rsa.generate_private_key(public_exponent=65537, key_size=key_size)
         elif key_spec.startswith("ECC"):
             curve = ECC_CURVES.get(key_spec)
-            self.key = ec.generate_private_key(curve)
+            key = ec.generate_private_key(curve)
         elif key_spec.startswith("HMAC"):
             if key_spec not in HMAC_RANGE_KEY_LENGTHS:
                 raise ValidationException(
                     f"1 validation error detected: Value '{key_spec}' at 'keySpec' "
                     f"failed to satisfy constraint: Member must satisfy enum value set: "
                     f"[RSA_2048, ECC_NIST_P384, ECC_NIST_P256, ECC_NIST_P521, HMAC_384, RSA_3072, "
                     f"ECC_SECG_P256K1, RSA_4096, SYMMETRIC_DEFAULT, HMAC_256, HMAC_224, HMAC_512]"
@@ -196,24 +188,32 @@
             self.key_material = os.urandom(random.randint(minimum_length, maximum_length))
             return
         else:
             # We do not support SM2 - asymmetric keys both suitable for ENCRYPT_DECRYPT and SIGN_VERIFY,
             # but only used in China AWS regions.
             raise UnsupportedOperationException(f"KeySpec {key_spec} is not supported")
 
-        self.private_key = self.key.private_bytes(
+        self.private_key = key.private_bytes(
             crypto_serialization.Encoding.DER,
             crypto_serialization.PrivateFormat.PKCS8,
             crypto_serialization.NoEncryption(),
         )
-        self.public_key = self.key.public_key().public_bytes(
+        self.public_key = key.public_key().public_bytes(
             crypto_serialization.Encoding.DER,
             crypto_serialization.PublicFormat.SubjectPublicKeyInfo,
         )
 
+    @property
+    def key(self) -> RSAPrivateKey:
+        return crypto_serialization.load_der_private_key(
+            self.private_key,
+            password=None,
+            backend=default_backend(),
+        )
+
 
 class KmsKey:
     metadata: KeyMetadata
     crypto_key: KmsCryptoKey
     tags: Dict[str, str]
     policy: str
     is_key_rotation_enabled: bool
@@ -609,22 +609,14 @@
 class KeyImportState:
     key_id: str
     import_token: str
     wrapping_algo: str
     key: KmsKey
 
 
-def validate_alias_name(alias_name: str) -> None:
-    if not alias_name.startswith("alias/"):
-        raise ValidationException(
-            'Alias must start with the prefix "alias/". Please see '
-            "https://docs.aws.amazon.com/kms/latest/developerguide/kms-alias.html"
-        )
-
-
 class KmsStore(BaseStore):
     # maps key ids to keys
     keys: Dict[str, KmsKey] = LocalAttribute(default=dict)
 
     # According to AWS documentation on grants https://docs.aws.amazon.com/kms/latest/APIReference/API_RetireGrant.html
     # "Cross-account use: Yes. You can retire a grant on a KMS key in a different AWS account."
 
@@ -639,149 +631,9 @@
 
     # maps key alias names to aliases
     aliases: Dict[str, KmsAlias] = LocalAttribute(default=dict)
 
     # maps import tokens to import data
     imports: Dict[str, KeyImportState] = LocalAttribute(default=dict)
 
-    # While in AWS keys have more than Enabled, Disabled and PendingDeletion states, we currently only model these 3
-    # in LocalStack, so this function is limited to them.
-    #
-    # The current default values are based on most of the operations working in AWS with enabled keys, but failing with
-    # disabled and those pending deletion.
-    #
-    # If we decide to use the other states as well, we might want to come up with a better key state validation per
-    # operation. Can consult this page for what states are supported by various operations:
-    # https://docs.aws.amazon.com/kms/latest/developerguide/key-state.html
-    def get_key(
-        self,
-        any_type_of_key_id: str,
-        any_key_state_allowed: bool = False,
-        enabled_key_allowed: bool = True,
-        disabled_key_allowed: bool = False,
-        pending_deletion_key_allowed: bool = False,
-    ) -> KmsKey:
-        if any_key_state_allowed:
-            enabled_key_allowed = True
-            disabled_key_allowed = True
-            pending_deletion_key_allowed = True
-        if not (enabled_key_allowed or disabled_key_allowed or pending_deletion_key_allowed):
-            raise ValueError("A key is requested, but all possible key states are prohibited")
-
-        key_id = self.get_key_id_from_any_id(any_type_of_key_id)
-
-        key = self.keys[key_id]
-        if not disabled_key_allowed and key.metadata.get("KeyState") == "Disabled":
-            raise DisabledException(f"{key.metadata.get('Arn')} is disabled.")
-        if not pending_deletion_key_allowed and key.metadata.get("KeyState") == "PendingDeletion":
-            raise KMSInvalidStateException(f"{key.metadata.get('Arn')} is pending deletion.")
-        if not enabled_key_allowed and key.metadata.get("KeyState") == "Enabled":
-            raise KMSInvalidStateException(
-                f"{key.metadata.get('Arn')} is enabled, but the operation doesn't support "
-                f"such a state"
-            )
-        return self.keys[key_id]
-
-    # TODO account_id and region params here are somewhat redundant, the store is supposed to know them. But at the
-    #  moment there is no way to get them from the store itself. Should get rid of these params later.
-    def get_alias(self, alias_name_or_arn: str, account_id: str, region: str) -> KmsAlias:
-        if not alias_name_or_arn.startswith("arn:"):
-            alias_name = alias_name_or_arn
-        else:
-            if ":alias/" not in alias_name_or_arn:
-                raise ValidationException(f"{alias_name_or_arn} is not a valid alias ARN")
-            alias_name = "alias/" + alias_name_or_arn.split(":alias/")[1]
-
-        validate_alias_name(alias_name)
-
-        if alias_name not in self.aliases:
-            alias_arn = kms_alias_arn(alias_name, account_id, region)
-            # AWS itself uses AliasArn instead of AliasName in this exception.
-            raise NotFoundException(f"Alias {alias_arn} is not found.")
-
-        return self.aliases.get(alias_name)
-
-    # Both account_id and region here are only supposed to be used to generate things like proper ARNs etc. The
-    # store for the key is not going to be selected using these parameters. Such a store selection is supposed to
-    # happen before the call to this function is made.
-    def create_key(
-        self, request: CreateKeyRequest = None, account_id: str = None, region: str = None
-    ):
-        key = KmsKey(request, account_id, region)
-        key_id = key.metadata.get("KeyId")
-        self.keys[key_id] = key
-        return key
-
-    # Both account_id and region here are only supposed to be used to generate things like proper ARNs etc. The
-    # store for the key is not going to be selected using these parameters. Such a store selection is supposed to
-    # happen before the call to this function is made.
-    def create_alias(self, request: CreateAliasRequest, account_id: str = None, region: str = None):
-        alias = KmsAlias(request, account_id, region)
-        alias_name = request.get("AliasName")
-        self.aliases[alias_name] = alias
-
-    # TODO Currently we follow the old moto implementation where reserved aliases and corresponding keys are getting
-    #  generated on the fly when someone tries to access such an alias. This is not great, as such aliases and keys
-    #  are not visible to ListAliases prior to someone trying to access such an alias. A better way might be to
-    #  generate all such aliases and keys the moment we initialize a new set of stores. But it might be an
-    #  unnecessary overhead. Should decide later, which approach is better.
-    def _create_alias_if_reserved_and_not_exists(
-        self, alias_name: str, account_id: str = None, region: str = None
-    ):
-        if alias_name not in RESERVED_ALIASES or alias_name in self.aliases:
-            return
-        create_key_request = {}
-        key_id = self.create_key(create_key_request, account_id, region).metadata.get("KeyId")
-        create_alias_request = CreateAliasRequest(AliasName=alias_name, TargetKeyId=key_id)
-        self.create_alias(create_alias_request, account_id, region)
-
-    # In KMS, keys can be identified by
-    # - key ID
-    # - key ARN
-    # - key alias
-    # - key alias' ARN
-    # This function allows us to find a key by any of these identifiers.
-    def get_key_id_from_any_id(
-        self, some_id: str, account_id: str = None, region: str = None
-    ) -> str:
-        alias_name = None
-        key_id = None
-        key_arn = None
-        if some_id.startswith("arn:"):
-            if ":alias/" in some_id:
-                alias_arn = some_id
-                alias_name = "alias/" + alias_arn.split(":alias/")[1]
-            elif ":key/" in some_id:
-                key_arn = some_id
-                key_id = key_arn.split(":key/")[1]
-                parsed_arn = parse_arn(key_arn)
-                if parsed_arn["region"] != self._region_name:
-                    raise NotFoundException(f"Invalid arn {parsed_arn['region']}")
-            else:
-                raise ValueError(
-                    f"Supplied value of {some_id} is an ARN, but neither of a KMS key nor of a KMS key "
-                    f"alias"
-                )
-        elif some_id.startswith("alias/"):
-            alias_name = some_id
-        else:
-            key_id = some_id
-
-        if alias_name:
-            self._create_alias_if_reserved_and_not_exists(alias_name, account_id, region)
-            if alias_name not in self.aliases:
-                raise NotFoundException(f"Unable to find KMS alias with name {alias_name}")
-            key_id = self.aliases[alias_name].metadata["TargetKeyId"]
-
-        # regular KeyId are UUID, and MultiRegion keys starts with 'mrk-' and 32 hex chars
-        if not PATTERN_UUID.match(key_id) and not MULTI_REGION_PATTERN.match(key_id):
-            raise NotFoundException(f"Invalid keyId {key_id}")
-
-        if key_id not in self.keys:
-            if not key_arn:
-                key_arn = f"arn:aws:kms:{self._region_name}:{self._account_id}:key/{key_id}"
-            raise NotFoundException(f"Key '{key_arn}' does not exist")
-
-        return key_id
-
 
 kms_stores = AccountRegionBundle("kms", KmsStore)
```

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     CreateKeyRequest,
     CreateKeyResponse,
     DateType,
     DecryptResponse,
     DeleteAliasRequest,
     DescribeKeyRequest,
     DescribeKeyResponse,
+    DisabledException,
     DisableKeyRequest,
     DisableKeyRotationRequest,
     EnableKeyRequest,
     EncryptionAlgorithmSpec,
     EncryptionContextType,
     EncryptResponse,
     ExpirationModelType,
@@ -95,28 +96,31 @@
     UpdateKeyDescriptionRequest,
     VerifyMacRequest,
     VerifyMacResponse,
     VerifyRequest,
     VerifyResponse,
     WrappingKeySpec,
 )
+from localstack.services.kms.exceptions import ValidationException
 from localstack.services.kms.models import (
+    MULTI_REGION_PATTERN,
+    PATTERN_UUID,
+    RESERVED_ALIASES,
     KeyImportState,
+    KmsAlias,
     KmsCryptoKey,
     KmsGrant,
     KmsKey,
     KmsStore,
-    ValidationException,
     deserialize_ciphertext_blob,
     kms_stores,
-    validate_alias_name,
 )
-from localstack.services.kms.utils import is_valid_key_arn, parse_key_arn
+from localstack.services.kms.utils import is_valid_key_arn, parse_key_arn, validate_alias_name
 from localstack.services.plugins import ServiceLifecycleHook
-from localstack.utils.aws.arns import kms_alias_arn
+from localstack.utils.aws.arns import kms_alias_arn, parse_arn
 from localstack.utils.collections import PaginatedList
 from localstack.utils.common import select_attributes
 from localstack.utils.strings import short_uid, to_bytes, to_str
 
 LOG = logging.getLogger(__name__)
 
 # valid operations
@@ -170,21 +174,172 @@
     - GenerateMac
     - ReEncrypt
     - Sign
     - Verify
     - VerifyMac
     """
 
+    #
+    # Helpers
+    #
+
     @staticmethod
     def _get_store(account_id: str, region_name: str) -> KmsStore:
         return kms_stores[account_id][region_name]
 
     @staticmethod
-    def _get_key(account_id: str, region_name: str, key_id: str, **kwargs) -> KmsKey:
-        return KmsProvider._get_store(account_id, region_name).get_key(key_id, **kwargs)
+    def _create_kms_alias(account_id: str, region_name: str, request: CreateAliasRequest):
+        store = kms_stores[account_id][region_name]
+        alias = KmsAlias(request, account_id, region_name)
+        alias_name = request.get("AliasName")
+        store.aliases[alias_name] = alias
+
+    @staticmethod
+    def _create_kms_key(
+        account_id: str, region_name: str, request: CreateKeyRequest = None
+    ) -> KmsKey:
+        store = kms_stores[account_id][region_name]
+        key = KmsKey(request, account_id, region_name)
+        key_id = key.metadata.get("KeyId")
+        store.keys[key_id] = key
+        return key
+
+    @staticmethod
+    def _get_key_id_from_any_id(account_id: str, region_name: str, some_id: str) -> str:
+        """
+        Resolve a KMS key ID by using one of the following identifiers:
+        - key ID
+        - key ARN
+        - key alias
+        - key alias ARN
+        """
+        alias_name = None
+        key_id = None
+        key_arn = None
+
+        if some_id.startswith("arn:"):
+            if ":alias/" in some_id:
+                alias_arn = some_id
+                alias_name = "alias/" + alias_arn.split(":alias/")[1]
+            elif ":key/" in some_id:
+                key_arn = some_id
+                key_id = key_arn.split(":key/")[1]
+                parsed_arn = parse_arn(key_arn)
+                if parsed_arn["region"] != region_name:
+                    raise NotFoundException(f"Invalid arn {parsed_arn['region']}")
+            else:
+                raise ValueError(
+                    f"Supplied value of {some_id} is an ARN, but neither of a KMS key nor of a KMS key "
+                    f"alias"
+                )
+        elif some_id.startswith("alias/"):
+            alias_name = some_id
+        else:
+            key_id = some_id
+
+        store = kms_stores[account_id][region_name]
+
+        if alias_name:
+            KmsProvider._create_alias_if_reserved_and_not_exists(
+                account_id,
+                region_name,
+                alias_name,
+            )
+            if alias_name not in store.aliases:
+                raise NotFoundException(f"Unable to find KMS alias with name {alias_name}")
+            key_id = store.aliases[alias_name].metadata["TargetKeyId"]
+
+        # regular KeyId are UUID, and MultiRegion keys starts with 'mrk-' and 32 hex chars
+        if not PATTERN_UUID.match(key_id) and not MULTI_REGION_PATTERN.match(key_id):
+            raise NotFoundException(f"Invalid keyId {key_id}")
+
+        if key_id not in store.keys:
+            if not key_arn:
+                key_arn = f"arn:aws:kms:{region_name}:{account_id}:key/{key_id}"
+            raise NotFoundException(f"Key '{key_arn}' does not exist")
+
+        return key_id
+
+    @staticmethod
+    def _create_alias_if_reserved_and_not_exists(
+        account_id: str, region_name: str, alias_name: str
+    ):
+        store = kms_stores[account_id][region_name]
+        if alias_name not in RESERVED_ALIASES or alias_name in store.aliases:
+            return
+        create_key_request = {}
+        key_id = KmsProvider._create_kms_key(
+            account_id,
+            region_name,
+            create_key_request,
+        ).metadata.get("KeyId")
+        create_alias_request = CreateAliasRequest(AliasName=alias_name, TargetKeyId=key_id)
+        KmsProvider._create_kms_alias(account_id, region_name, create_alias_request)
+
+    # While in AWS keys have more than Enabled, Disabled and PendingDeletion states, we currently only model these 3
+    # in LocalStack, so this function is limited to them.
+    #
+    # The current default values are based on most of the operations working in AWS with enabled keys, but failing with
+    # disabled and those pending deletion.
+    #
+    # If we decide to use the other states as well, we might want to come up with a better key state validation per
+    # operation. Can consult this page for what states are supported by various operations:
+    # https://docs.aws.amazon.com/kms/latest/developerguide/key-state.html
+    @staticmethod
+    def _get_kms_key(
+        account_id: str,
+        region_name: str,
+        any_type_of_key_id: str,
+        any_key_state_allowed: bool = False,
+        enabled_key_allowed: bool = True,
+        disabled_key_allowed: bool = False,
+        pending_deletion_key_allowed: bool = False,
+    ) -> KmsKey:
+        store = kms_stores[account_id][region_name]
+
+        if any_key_state_allowed:
+            enabled_key_allowed = True
+            disabled_key_allowed = True
+            pending_deletion_key_allowed = True
+        if not (enabled_key_allowed or disabled_key_allowed or pending_deletion_key_allowed):
+            raise ValueError("A key is requested, but all possible key states are prohibited")
+
+        key_id = KmsProvider._get_key_id_from_any_id(account_id, region_name, any_type_of_key_id)
+        key = store.keys[key_id]
+
+        if not disabled_key_allowed and key.metadata.get("KeyState") == "Disabled":
+            raise DisabledException(f"{key.metadata.get('Arn')} is disabled.")
+        if not pending_deletion_key_allowed and key.metadata.get("KeyState") == "PendingDeletion":
+            raise KMSInvalidStateException(f"{key.metadata.get('Arn')} is pending deletion.")
+        if not enabled_key_allowed and key.metadata.get("KeyState") == "Enabled":
+            raise KMSInvalidStateException(
+                f"{key.metadata.get('Arn')} is enabled, but the operation doesn't support "
+                f"such a state"
+            )
+        return store.keys[key_id]
+
+    @staticmethod
+    def _get_kms_alias(account_id: str, region_name: str, alias_name_or_arn: str) -> KmsAlias:
+        store = kms_stores[account_id][region_name]
+
+        if not alias_name_or_arn.startswith("arn:"):
+            alias_name = alias_name_or_arn
+        else:
+            if ":alias/" not in alias_name_or_arn:
+                raise ValidationException(f"{alias_name_or_arn} is not a valid alias ARN")
+            alias_name = "alias/" + alias_name_or_arn.split(":alias/")[1]
+
+        validate_alias_name(alias_name)
+
+        if alias_name not in store.aliases:
+            alias_arn = kms_alias_arn(alias_name, account_id, region_name)
+            # AWS itself uses AliasArn instead of AliasName in this exception.
+            raise NotFoundException(f"Alias {alias_arn} is not found.")
+
+        return store.aliases.get(alias_name)
 
     @staticmethod
     def _parse_key_id(key_id_or_arn: str, context: RequestContext) -> Tuple[str, str, str]:
         """
         Return locator attributes (account ID, region_name, key ID) of a given KMS key.
 
         If an ARN is provided, this is extracted from it. Otherwise, context data is used.
@@ -197,35 +352,37 @@
             account_id, region_name, key_id = parse_key_arn(key_id_or_arn)
             if region_name != context.region:
                 raise NotFoundException(f"Invalid arn {region_name}")
             return account_id, region_name, key_id
 
         return context.account_id, context.region, key_id_or_arn
 
+    #
+    # Operation Handlers
+    #
+
     @handler("CreateKey", expand=False)
     def create_key(
         self,
         context: RequestContext,
         request: CreateKeyRequest = None,
     ) -> CreateKeyResponse:
-        key = self._get_store(context.account_id, context.region).create_key(
-            request, context.account_id, context.region
-        )
+        key = self._create_kms_key(context.account_id, context.region, request)
         return CreateKeyResponse(KeyMetadata=key.metadata)
 
     @handler("ScheduleKeyDeletion", expand=False)
     def schedule_key_deletion(
         self, context: RequestContext, request: ScheduleKeyDeletionRequest
     ) -> ScheduleKeyDeletionResponse:
         pending_window = int(request.get("PendingWindowInDays", 30))
         if pending_window < 7 or pending_window > 30:
             raise ValidationException(
                 f"PendingWindowInDays should be between 7 and 30, but it is {pending_window}"
             )
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id,
             context.region,
             request.get("KeyId"),
             enabled_key_allowed=True,
             disabled_key_allowed=True,
         )
         key.schedule_key_deletion(pending_window)
@@ -234,15 +391,15 @@
         result["PendingWindowInDays"] = pending_window
         return ScheduleKeyDeletionResponse(**result)
 
     @handler("CancelKeyDeletion", expand=False)
     def cancel_key_deletion(
         self, context: RequestContext, request: CancelKeyDeletionRequest
     ) -> CancelKeyDeletionResponse:
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id,
             context.region,
             request.get("KeyId"),
             enabled_key_allowed=False,
             pending_deletion_key_allowed=True,
         )
         key.metadata["KeyState"] = KeyState.Disabled
@@ -250,27 +407,27 @@
         # https://docs.aws.amazon.com/kms/latest/APIReference/API_CancelKeyDeletion.html#API_CancelKeyDeletion_ResponseElements
         # "The Amazon Resource Name (key ARN) of the KMS key whose deletion is canceled."
         return CancelKeyDeletionResponse(KeyId=key.metadata.get("Arn"))
 
     @handler("DisableKey", expand=False)
     def disable_key(self, context: RequestContext, request: DisableKeyRequest) -> None:
         # Technically, AWS allows DisableKey for keys that are already disabled.
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id,
             context.region,
             request.get("KeyId"),
             enabled_key_allowed=True,
             disabled_key_allowed=True,
         )
         key.metadata["KeyState"] = KeyState.Disabled
         key.metadata["Enabled"] = False
 
     @handler("EnableKey", expand=False)
     def enable_key(self, context: RequestContext, request: EnableKeyRequest) -> None:
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id,
             context.region,
             request.get("KeyId"),
             enabled_key_allowed=True,
             disabled_key_allowed=True,
         )
         key.metadata["KeyState"] = KeyState.Enabled
@@ -297,23 +454,22 @@
         return ListKeysResponse(Keys=page, **kwargs)
 
     @handler("DescribeKey", expand=False)
     def describe_key(
         self, context: RequestContext, request: DescribeKeyRequest
     ) -> DescribeKeyResponse:
         account_id, region_name, key_id = self._parse_key_id(request["KeyId"], context)
-        key = self._get_key(account_id, region_name, key_id, any_key_state_allowed=True)
+        key = self._get_kms_key(account_id, region_name, key_id, any_key_state_allowed=True)
         return DescribeKeyResponse(KeyMetadata=key.metadata)
 
     @handler("ReplicateKey", expand=False)
     def replicate_key(
         self, context: RequestContext, request: ReplicateKeyRequest
     ) -> ReplicateKeyResponse:
-        replicate_from_store = self._get_store(context.account_id, context.region)
-        key = replicate_from_store.get_key(request.get("KeyId"))
+        key = self._get_kms_key(context.account_id, context.region, request.get("KeyId"))
         key_id = key.metadata.get("KeyId")
         if not key.metadata.get("MultiRegion"):
             raise UnsupportedOperationException(
                 f"Unable to replicate a non-MultiRegion key {key_id}"
             )
         replica_region = request.get("ReplicaRegion")
         replicate_to_store = kms_stores[context.account_id][replica_region]
@@ -330,30 +486,29 @@
         replicate_to_store.keys[key_id] = replica_key
         return ReplicateKeyResponse(ReplicaKeyMetadata=replica_key.metadata)
 
     @handler("UpdateKeyDescription", expand=False)
     def update_key_description(
         self, context: RequestContext, request: UpdateKeyDescriptionRequest
     ) -> None:
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id,
             context.region,
             request.get("KeyId"),
             enabled_key_allowed=True,
             disabled_key_allowed=True,
         )
         key.metadata["Description"] = request.get("Description")
 
     @handler("CreateGrant", expand=False)
     def create_grant(
         self, context: RequestContext, request: CreateGrantRequest
     ) -> CreateGrantResponse:
         key_account_id, key_region_name, key_id = self._parse_key_id(request["KeyId"], context)
-        store_kms_key = self._get_store(key_account_id, key_region_name)
-        key = store_kms_key.get_key(key_id)
+        key = self._get_kms_key(key_account_id, key_region_name, key_id)
 
         # KeyId can potentially hold one of multiple different types of key identifiers. Here we find a key no
         # matter which type of id is used.
         key_id = key.metadata.get("KeyId")
         request["KeyId"] = key_id
         self._validate_grant_request(request)
         grant_name = request.get("Name")
@@ -381,18 +536,19 @@
     @handler("ListGrants", expand=False)
     def list_grants(
         self, context: RequestContext, request: ListGrantsRequest
     ) -> ListGrantsResponse:
         if not request.get("KeyId"):
             raise ValidationError("Required input parameter KeyId not specified")
         key_account_id, key_region_name, _ = self._parse_key_id(request["KeyId"], context)
-        key_store = self._get_store(key_account_id, key_region_name)
         # KeyId can potentially hold one of multiple different types of key identifiers. Here we find a key no
         # matter which type of id is used.
-        key = key_store.get_key(request.get("KeyId"), any_key_state_allowed=True)
+        key = self._get_kms_key(
+            key_account_id, key_region_name, request.get("KeyId"), any_key_state_allowed=True
+        )
         key_id = key.metadata.get("KeyId")
 
         store = self._get_store(context.account_id, context.region)
         grant_id = request.get("GrantId")
         if grant_id:
             if grant_id not in store.grants:
                 raise InvalidGrantIdException()
@@ -433,17 +589,15 @@
         store.grant_names.pop((grant.metadata.get("Name"), key_id), None)
         store.grants.pop(grant_id)
 
     def revoke_grant(
         self, context: RequestContext, key_id: KeyIdType, grant_id: GrantIdType
     ) -> None:
         key_account_id, key_region_name, key_id = self._parse_key_id(key_id, context)
-        key = self._get_store(key_account_id, key_region_name).get_key(
-            key_id, any_key_state_allowed=True
-        )
+        key = self._get_kms_key(key_account_id, key_region_name, key_id, any_key_state_allowed=True)
         key_id = key.metadata.get("KeyId")
 
         store = self._get_store(context.account_id, context.region)
 
         if grant_id not in store.grants:
             raise InvalidGrantIdException()
 
@@ -469,16 +623,17 @@
 
             grant_id = grant_store.grant_tokens[grant_token]
         else:
             grant_store = self._get_store(context.account_id, context.region)
 
         if key_id:
             key_account_id, key_region_name, key_id = self._parse_key_id(key_id, context)
-            key_store = self._get_store(key_account_id, key_region_name)
-            key = key_store.get_key(key_id, any_key_state_allowed=True)
+            key = self._get_kms_key(
+                key_account_id, key_region_name, key_id, any_key_state_allowed=True
+            )
             key_id = key.metadata.get("KeyId")
         else:
             _, _, key_id = parse_key_arn(grant_store.grants[grant_id].metadata.get("KeyArn"))
 
         self._delete_grant(grant_store, grant_id, key_id)
 
     def list_retirable_grants(
@@ -509,15 +664,15 @@
 
     def get_public_key(
         self, context: RequestContext, key_id: KeyIdType, grant_tokens: GrantTokenList = None
     ) -> GetPublicKeyResponse:
         # According to https://docs.aws.amazon.com/kms/latest/developerguide/key-state.html, GetPublicKey is supposed
         # to fail for disabled keys. But it actually doesn't fail in AWS.
         account_id, region_name, key_id = self._parse_key_id(key_id, context)
-        key = self._get_key(
+        key = self._get_kms_key(
             account_id,
             region_name,
             key_id,
             enabled_key_allowed=True,
             disabled_key_allowed=True,
         )
         attrs = [
@@ -529,15 +684,15 @@
         result = select_attributes(key.metadata, attrs)
         result["PublicKey"] = key.crypto_key.public_key
         result["KeyId"] = key.metadata["Arn"]
         return GetPublicKeyResponse(**result)
 
     def _generate_data_key_pair(self, key_id: str, key_pair_spec: str, context: RequestContext):
         account_id, region_name, key_id = self._parse_key_id(key_id, context)
-        key = self._get_key(account_id, region_name, key_id)
+        key = self._get_kms_key(account_id, region_name, key_id)
         self._validate_key_for_encryption_decryption(context, key)
         crypto_key = KmsCryptoKey(key_pair_spec)
         return {
             "KeyId": key.metadata["Arn"],
             "KeyPairSpec": key_pair_spec,
             "PrivateKeyCiphertextBlob": key.encrypt(crypto_key.private_key),
             "PrivateKeyPlaintext": crypto_key.private_key,
@@ -591,15 +746,15 @@
     # KeySpec for CreateKey) nor on NumberOfBytes. Instead, we generate a key with a key length that is "standard" in
     # LocalStack.
     #
     def _generate_data_key(
         self, context: RequestContext, key_id: str, encryption_context: EncryptionContextType = None
     ):
         account_id, region_name, key_id = self._parse_key_id(key_id, context)
-        key = self._get_key(account_id, region_name, key_id)
+        key = self._get_kms_key(account_id, region_name, key_id)
         # TODO Should also have a validation for the key being a symmetric one.
         self._validate_key_for_encryption_decryption(context, key)
         crypto_key = KmsCryptoKey("SYMMETRIC_DEFAULT")
         return {
             "KeyId": key.metadata["Arn"],
             "Plaintext": crypto_key.key_material,
             "CiphertextBlob": key.encrypt(crypto_key.key_material, encryption_context),
@@ -630,15 +785,15 @@
         context: RequestContext,
         request: GenerateMacRequest,
     ) -> GenerateMacResponse:
         msg = request.get("Message")
         self._validate_mac_msg_length(msg)
 
         account_id, region_name, key_id = self._parse_key_id(request["KeyId"], context)
-        key = self._get_key(account_id, region_name, key_id)
+        key = self._get_kms_key(account_id, region_name, key_id)
 
         self._validate_key_for_generate_verify_mac(context, key)
 
         algorithm = request.get("MacAlgorithm")
         self._validate_mac_algorithm(key, algorithm)
 
         mac = key.generate_mac(msg, algorithm)
@@ -651,15 +806,15 @@
         context: RequestContext,
         request: VerifyMacRequest,
     ) -> VerifyMacResponse:
         msg = request.get("Message")
         self._validate_mac_msg_length(msg)
 
         account_id, region_name, key_id = self._parse_key_id(request["KeyId"], context)
-        key = self._get_key(account_id, region_name, key_id)
+        key = self._get_kms_key(account_id, region_name, key_id)
 
         self._validate_key_for_generate_verify_mac(context, key)
 
         algorithm = request.get("MacAlgorithm")
         self._validate_mac_algorithm(key, algorithm)
 
         mac_valid = key.verify_mac(msg, request.get("Mac"), algorithm)
@@ -667,15 +822,15 @@
         return VerifyMacResponse(
             KeyId=key.metadata.get("Arn"), MacValid=mac_valid, MacAlgorithm=algorithm
         )
 
     @handler("Sign", expand=False)
     def sign(self, context: RequestContext, request: SignRequest) -> SignResponse:
         account_id, region_name, key_id = self._parse_key_id(request["KeyId"], context)
-        key = self._get_key(account_id, region_name, key_id)
+        key = self._get_kms_key(account_id, region_name, key_id)
 
         self._validate_key_for_sign_verify(context, key)
 
         # TODO Add constraints on KeySpec / SigningAlgorithm pairs:
         #  https://docs.aws.amazon.com/kms/latest/developerguide/asymmetric-key-specs.html#key-spec-ecc
 
         signing_algorithm = request.get("SigningAlgorithm")
@@ -688,15 +843,15 @@
         }
         return SignResponse(**result)
 
     # Currently LocalStack only calculates SHA256 digests no matter what the signing algorithm is.
     @handler("Verify", expand=False)
     def verify(self, context: RequestContext, request: VerifyRequest) -> VerifyResponse:
         account_id, region_name, key_id = self._parse_key_id(request["KeyId"], context)
-        key = self._get_key(account_id, region_name, key_id)
+        key = self._get_kms_key(account_id, region_name, key_id)
 
         self._validate_key_for_sign_verify(context, key)
 
         signing_algorithm = request.get("SigningAlgorithm")
         is_signature_valid = key.verify(
             request.get("Message"),
             request.get("MessageType"),
@@ -732,15 +887,15 @@
         key_id: KeyIdType,
         plaintext: PlaintextType,
         encryption_context: EncryptionContextType = None,
         grant_tokens: GrantTokenList = None,
         encryption_algorithm: EncryptionAlgorithmSpec = None,
     ) -> EncryptResponse:
         account_id, region_name, key_id = self._parse_key_id(key_id, context)
-        key = self._get_key(account_id, region_name, key_id)
+        key = self._get_kms_key(account_id, region_name, key_id)
         self._validate_plaintext_length(plaintext)
         self._validate_plaintext_key_type_based(plaintext, key, encryption_algorithm)
         self._validate_key_for_encryption_decryption(context, key)
         self._validate_key_state_not_pending_import(key)
 
         ciphertext_blob = key.encrypt(plaintext, encryption_context)
         # For compatibility, we return EncryptionAlgorithm values expected from AWS. But LocalStack currently always
@@ -771,15 +926,15 @@
             ciphertext = deserialize_ciphertext_blob(ciphertext_blob=ciphertext_blob)
         except Exception:
             raise InvalidCiphertextException(
                 "LocalStack is unable to deserialize the ciphertext blob. Perhaps the "
                 "blob didn't come from LocalStack"
             )
         account_id, region_name, key_id = self._parse_key_id(key_id or ciphertext.key_id, context)
-        key = self._get_key(account_id, region_name, key_id)
+        key = self._get_kms_key(account_id, region_name, key_id)
         if key.metadata["KeyId"] != ciphertext.key_id:
             raise IncorrectKeyException(
                 "The key ID in the request does not identify a CMK that can perform this operation."
             )
 
         self._validate_key_for_encryption_decryption(context, key)
         self._validate_key_state_not_pending_import(key)
@@ -807,16 +962,20 @@
         key_id: KeyIdType,
         wrapping_algorithm: AlgorithmSpec,
         wrapping_key_spec: WrappingKeySpec,
     ) -> GetParametersForImportResponse:
         store = self._get_store(context.account_id, context.region)
         # KeyId can potentially hold one of multiple different types of key identifiers. get_key finds a key no
         # matter which type of id is used.
-        key_to_import_material_to = store.get_key(
-            key_id, enabled_key_allowed=True, disabled_key_allowed=True
+        key_to_import_material_to = self._get_kms_key(
+            context.account_id,
+            context.region,
+            key_id,
+            enabled_key_allowed=True,
+            disabled_key_allowed=True,
         )
         if key_to_import_material_to.metadata.get("Origin") != "EXTERNAL":
             raise UnsupportedOperationException(
                 "Key material can only be imported into keys with Origin of EXTERNAL"
             )
         self._validate_key_for_encryption_decryption(context, key_to_import_material_to)
         key_id = key_to_import_material_to.metadata["KeyId"]
@@ -848,16 +1007,20 @@
         expiration_model: ExpirationModelType = None,
     ) -> ImportKeyMaterialResponse:
         store = self._get_store(context.account_id, context.region)
         import_token = to_str(import_token)
         import_state = store.imports.get(import_token)
         if not import_state:
             raise NotFoundException(f"Unable to find key import token '{import_token}'")
-        key_to_import_material_to = store.get_key(
-            key_id, enabled_key_allowed=True, disabled_key_allowed=True
+        key_to_import_material_to = self._get_kms_key(
+            context.account_id,
+            context.region,
+            key_id,
+            enabled_key_allowed=True,
+            disabled_key_allowed=True,
         )
         self._validate_key_for_encryption_decryption(context, key_to_import_material_to)
 
         if import_state.wrapping_algo == AlgorithmSpec.RSAES_PKCS1_V1_5:
             decrypt_padding = padding.PKCS1v15()
         elif import_state.wrapping_algo == AlgorithmSpec.RSAES_OAEP_SHA_1:
             decrypt_padding = padding.OAEP(padding.MGF1(hashes.SHA1()), hashes.SHA1(), None)
@@ -890,16 +1053,21 @@
         # TODO actually set validTo and make the key expire
         key_to_import_material_to.crypto_key.key_material = key_material
         key_to_import_material_to.metadata["Enabled"] = True
         key_to_import_material_to.metadata["KeyState"] = KeyState.Enabled
         return ImportKeyMaterialResponse()
 
     def delete_imported_key_material(self, context: RequestContext, key_id: KeyIdType) -> None:
-        store = self._get_store(context.account_id, context.region)
-        key = store.get_key(key_id, enabled_key_allowed=True, disabled_key_allowed=True)
+        key = self._get_kms_key(
+            context.account_id,
+            context.region,
+            key_id,
+            enabled_key_allowed=True,
+            disabled_key_allowed=True,
+        )
         key.crypto_key.key_material = None
         key.metadata["Enabled"] = False
         key.metadata["KeyState"] = KeyState.PendingImport
         key.metadata.pop("ExpirationModel", None)
 
     @handler("CreateAlias", expand=False)
     def create_alias(self, context: RequestContext, request: CreateAliasRequest) -> None:
@@ -908,23 +1076,23 @@
         validate_alias_name(alias_name)
         if alias_name in store.aliases:
             alias_arn = store.aliases.get(alias_name).metadata["AliasArn"]
             # AWS itself uses AliasArn instead of AliasName in this exception.
             raise AlreadyExistsException(f"An alias with the name {alias_arn} already exists")
         # KeyId can potentially hold one of multiple different types of key identifiers. Here we find a key no
         # matter which type of id is used.
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id,
             context.region,
             request.get("TargetKeyId"),
             enabled_key_allowed=True,
             disabled_key_allowed=True,
         )
         request["TargetKeyId"] = key.metadata.get("KeyId")
-        store.create_alias(request)
+        self._create_kms_alias(context.account_id, context.region, request)
 
     @handler("DeleteAlias", expand=False)
     def delete_alias(self, context: RequestContext, request: DeleteAliasRequest) -> None:
         # We do not check the state of the key, as, according to AWS docs, all key states, that are possible in
         # LocalStack, are supported by this operation.
         store = self._get_store(context.account_id, context.region)
         alias_name = request["AliasName"]
@@ -942,19 +1110,24 @@
         # Also disabled keys are accepted for this operation (see the table on that page).
         #
         # As such, we do not care about the state of the source key, but check the destination one.
 
         alias_name = request["AliasName"]
         # This API, per AWS docs, accepts only names, not ARNs.
         validate_alias_name(alias_name)
-        store = self._get_store(context.account_id, context.region)
-        alias = store.get_alias(alias_name, context.account_id, context.region)
+        alias = self._get_kms_alias(context.account_id, context.region, alias_name)
         key_id = request["TargetKeyId"]
         # Don't care about the key itself, just want to validate its state.
-        store.get_key(key_id, enabled_key_allowed=True, disabled_key_allowed=True)
+        self._get_kms_key(
+            context.account_id,
+            context.region,
+            key_id,
+            enabled_key_allowed=True,
+            disabled_key_allowed=True,
+        )
         alias.metadata["TargetKeyId"] = key_id
         alias.update_date_of_last_update()
 
     @handler("ListAliases")
     def list_aliases(
         self,
         context: RequestContext,
@@ -962,15 +1135,17 @@
         limit: LimitType = None,
         marker: MarkerType = None,
     ) -> ListAliasesResponse:
         store = self._get_store(context.account_id, context.region)
         if key_id:
             # KeyId can potentially hold one of multiple different types of key identifiers. Here we find a key no
             # matter which type of id is used.
-            key = store.get_key(key_id, any_key_state_allowed=True)
+            key = self._get_kms_key(
+                context.account_id, context.region, key_id, any_key_state_allowed=True
+            )
             key_id = key.metadata.get("KeyId")
 
         matching_aliases = []
         for alias in store.aliases.values():
             if key_id and alias.metadata["TargetKeyId"] != key_id:
                 continue
             matching_aliases.append(alias.metadata)
@@ -988,74 +1163,74 @@
     def get_key_rotation_status(
         self, context: RequestContext, request: GetKeyRotationStatusRequest
     ) -> GetKeyRotationStatusResponse:
         # https://docs.aws.amazon.com/kms/latest/developerguide/key-state.html
         # "If the KMS key has imported key material or is in a custom key store: UnsupportedOperationException."
         # We do not model that here, though.
         account_id, region_name, key_id = self._parse_key_id(request["KeyId"], context)
-        key = self._get_key(account_id, region_name, key_id, any_key_state_allowed=True)
+        key = self._get_kms_key(account_id, region_name, key_id, any_key_state_allowed=True)
         return GetKeyRotationStatusResponse(KeyRotationEnabled=key.is_key_rotation_enabled)
 
     @handler("DisableKeyRotation", expand=False)
     def disable_key_rotation(
         self, context: RequestContext, request: DisableKeyRotationRequest
     ) -> None:
         # https://docs.aws.amazon.com/kms/latest/developerguide/key-state.html
         # "If the KMS key has imported key material or is in a custom key store: UnsupportedOperationException."
         # We do not model that here, though.
-        key = self._get_key(context.account_id, context.region, request.get("KeyId"))
+        key = self._get_kms_key(context.account_id, context.region, request.get("KeyId"))
         key.is_key_rotation_enabled = False
 
     @handler("EnableKeyRotation", expand=False)
     def enable_key_rotation(
         self, context: RequestContext, request: DisableKeyRotationRequest
     ) -> None:
         # https://docs.aws.amazon.com/kms/latest/developerguide/key-state.html
         # "If the KMS key has imported key material or is in a custom key store: UnsupportedOperationException."
         # We do not model that here, though.
-        key = self._get_key(context.account_id, context.region, request.get("KeyId"))
+        key = self._get_kms_key(context.account_id, context.region, request.get("KeyId"))
         key.is_key_rotation_enabled = True
 
     @handler("ListKeyPolicies", expand=False)
     def list_key_policies(
         self, context: RequestContext, request: ListKeyPoliciesRequest
     ) -> ListKeyPoliciesResponse:
         # We just care if the key exists. The response, by AWS specifications, is the same for all keys, as the only
         # supported policy is "default":
         # https://docs.aws.amazon.com/kms/latest/APIReference/API_ListKeyPolicies.html#API_ListKeyPolicies_ResponseElements
-        self._get_key(
+        self._get_kms_key(
             context.account_id, context.region, request.get("KeyId"), any_key_state_allowed=True
         )
         return ListKeyPoliciesResponse(PolicyNames=["default"], Truncated=False)
 
     @handler("PutKeyPolicy", expand=False)
     def put_key_policy(self, context: RequestContext, request: PutKeyPolicyRequest) -> None:
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id, context.region, request.get("KeyId"), any_key_state_allowed=True
         )
         if request.get("PolicyName") != "default":
             raise UnsupportedOperationException("Only default policy is supported")
         key.policy = request.get("Policy")
 
     @handler("GetKeyPolicy", expand=False)
     def get_key_policy(
         self, context: RequestContext, request: GetKeyPolicyRequest
     ) -> GetKeyPolicyResponse:
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id, context.region, request.get("KeyId"), any_key_state_allowed=True
         )
         if request.get("PolicyName") != "default":
             raise NotFoundException("No such policy exists")
         return GetKeyPolicyResponse(Policy=key.policy)
 
     @handler("ListResourceTags", expand=False)
     def list_resource_tags(
         self, context: RequestContext, request: ListResourceTagsRequest
     ) -> ListResourceTagsResponse:
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id, context.region, request.get("KeyId"), any_key_state_allowed=True
         )
         keys_list = PaginatedList(
             [{"TagKey": tag_key, "TagValue": tag_value} for tag_key, tag_value in key.tags.items()]
         )
         page, next_token = keys_list.get_page(
             lambda tag: tag.get("TagKey"),
@@ -1063,26 +1238,26 @@
             page_size=request.get("Limit", 50),
         )
         kwargs = {"NextMarker": next_token, "Truncated": True} if next_token else {}
         return ListResourceTagsResponse(Tags=page, **kwargs)
 
     @handler("TagResource", expand=False)
     def tag_resource(self, context: RequestContext, request: TagResourceRequest) -> None:
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id,
             context.region,
             request.get("KeyId"),
             enabled_key_allowed=True,
             disabled_key_allowed=True,
         )
         key.add_tags(request.get("Tags"))
 
     @handler("UntagResource", expand=False)
     def untag_resource(self, context: RequestContext, request: UntagResourceRequest) -> None:
-        key = self._get_key(
+        key = self._get_kms_key(
             context.account_id,
             context.region,
             request.get("KeyId"),
             enabled_key_allowed=True,
             disabled_key_allowed=True,
         )
         if not request.get("TagKeys"):
@@ -1209,11 +1384,10 @@
 # Different AWS services have some internal integrations with KMS. Some create keys, that are used to encrypt/decrypt
 # customer's data. Such keys can't be created from outside for security reasons. So AWS services use some internal
 # APIs to do that. Functions here are supposed to be used by other LocalStack services to have similar integrations
 # with KMS in LocalStack. As such, they are supposed to be proper APIs (as in error and security handling),
 # just with more features.
 
 
-def set_key_managed(key_id: str, account_id: str, region: str) -> None:
-    store = kms_stores[account_id][region]
-    key = store.get_key(key_id)
+def set_key_managed(key_id: str, account_id: str, region_name: str) -> None:
+    key = KmsProvider._get_kms_key(account_id, region_name, key_id)
     key.metadata["KeyManager"] = "AWS"
```

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from typing import Tuple
 
+from localstack.services.kms.exceptions import ValidationException
+
 KMS_KEY_ARN_PATTERN = re.compile(
     r"^arn:aws:kms:(?P<region_name>[^:]+):(?P<account_id>\d{12}):key\/(?P<key_id>[^:]+)$"
 )
 
 
 def get_hash_algorithm(signing_algorithm: str) -> str:
     """
@@ -25,7 +27,15 @@
 
 
 def is_valid_key_arn(key_arn: str) -> bool:
     """
     Check if a given string is a valid KMS key ARN.
     """
     return KMS_KEY_ARN_PATTERN.match(key_arn) is not None
+
+
+def validate_alias_name(alias_name: str) -> None:
+    if not alias_name.startswith("alias/"):
+        raise ValidationException(
+            'Alias must start with the prefix "alias/". Please see '
+            "https://docs.aws.amazon.com/kms/latest/developerguide/kms-alias.html"
+        )
```

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/state/core.py` & `localstack-core-2.1.1.dev20230616121558/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230616121558/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230616121558/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230616121558/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/collections.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230616121558/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230616110406
+Version: 2.1.1.dev20230616121558
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,15 @@
 localstack/services/kinesis/kinesis_mock_server.py
 localstack/services/kinesis/kinesis_starter.py
 localstack/services/kinesis/models.py
 localstack/services/kinesis/packages.py
 localstack/services/kinesis/plugins.py
 localstack/services/kinesis/provider.py
 localstack/services/kms/__init__.py
+localstack/services/kms/exceptions.py
 localstack/services/kms/local_kms_provider.py
 localstack/services/kms/local_kms_server.py
 localstack/services/kms/models.py
 localstack/services/kms/packages.py
 localstack/services/kms/plugins.py
 localstack/services/kms/provider.py
 localstack/services/kms/utils.py
```

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8791666666666668%*

 * *Differences: {"'localstack.hooks.on_infra_shutdown'": '{insert: [(1, '*

 * *                                         "'_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown')], "*

 * *                                         'delete: [0]}',*

 * * "'localstack.hooks.on_infra_start'": '{insert: [(2, '*

 * *                                      "'_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser'), "*

 * *                                      '(3, '*

 * *                                      "'v […]*

```diff
@@ -49,40 +49,40 @@
         "configure_edge_port=localstack.plugins:configure_edge_port"
     ],
     "localstack.hooks.on_infra_ready": [
         "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
         "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
-        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
+        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
     ],
     "localstack.hooks.on_infra_start": [
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser"
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
         "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
-        "terraform/community=localstack.packages.plugins:terraform_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package"
+        "terraform/community=localstack.packages.plugins:terraform_package"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230616110406/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/pyproject.toml` & `localstack-core-2.1.1.dev20230616121558/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616110406/setup.cfg` & `localstack-core-2.1.1.dev20230616121558/setup.cfg`

 * *Files identical despite different names*

