# Comparing `tmp/localstack-core-2.1.1.dev20230616121558.tar.gz` & `tmp/localstack-core-2.1.1.dev20230616132853.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230616121558.tar", last modified: Fri Jun 16 12:16:05 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230616132853.tar", last modified: Fri Jun 16 13:29:01 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230616121558.tar` & `localstack-core-2.1.1.dev20230616132853.tar`

### file list

```diff
@@ -1,852 +1,856 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.609835 localstack-core-2.1.1.dev20230616121558/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-16 12:16:05.609835 localstack-core-2.1.1.dev20230616121558/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.521837 localstack-core-2.1.1.dev20230616121558/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.521837 localstack-core-2.1.1.dev20230616121558/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-16 12:15:58.000000 localstack-core-2.1.1.dev20230616121558/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.521837 localstack-core-2.1.1.dev20230616121558/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   755634 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.525837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.529837 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.533837 localstack-core-2.1.1.dev20230616121558/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    61609 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14059 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.537837 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.541837 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65108 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33005 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20991 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7434 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2190 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21924 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2949 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3188 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9196 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28213 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3327 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4787 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2640 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13639 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6708 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8678 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5134 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3927 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5754 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5500 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.545837 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59474 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.549836 localstack-core-2.1.1.dev20230616121558/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.553836 localstack-core-2.1.1.dev20230616121558/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43901 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.557836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.561836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.565836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.569836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.573836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.577836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.585836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.585836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.585836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.589836 localstack-core-2.1.1.dev20230616121558/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.597835 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.601835 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69752 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.601835 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.601835 localstack-core-2.1.1.dev20230616121558/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.605835 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:16:05.609835 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37846 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 12:16:02.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-16 12:16:02.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-16 12:16:05.000000 localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-16 12:16:05.609835 localstack-core-2.1.1.dev20230616121558/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-16 11:39:28.000000 localstack-core-2.1.1.dev20230616121558/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.994861 localstack-core-2.1.1.dev20230616132853/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-16 13:29:01.994861 localstack-core-2.1.1.dev20230616132853/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.886862 localstack-core-2.1.1.dev20230616132853/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-16 13:28:53.000000 localstack-core-2.1.1.dev20230616132853/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   755634 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.890862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.894862 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.898862 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.898862 localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.898862 localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.898862 localstack-core-2.1.1.dev20230616132853/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.898862 localstack-core-2.1.1.dev20230616132853/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.898862 localstack-core-2.1.1.dev20230616132853/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.898862 localstack-core-2.1.1.dev20230616132853/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.902862 localstack-core-2.1.1.dev20230616132853/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.902862 localstack-core-2.1.1.dev20230616132853/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.902862 localstack-core-2.1.1.dev20230616132853/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.902862 localstack-core-2.1.1.dev20230616132853/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.902862 localstack-core-2.1.1.dev20230616132853/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.902862 localstack-core-2.1.1.dev20230616132853/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.906862 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61609 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14059 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.906862 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.906862 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.906862 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.906862 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.910862 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.910862 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65108 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33005 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20991 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7434 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2190 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21924 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2949 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3188 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9196 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28213 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3327 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4787 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2640 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13639 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6708 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8678 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5134 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3927 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5754 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5500 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.914862 localstack-core-2.1.1.dev20230616132853/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.918861 localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.918861 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59474 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.918861 localstack-core-2.1.1.dev20230616132853/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.918861 localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.918861 localstack-core-2.1.1.dev20230616132853/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.918861 localstack-core-2.1.1.dev20230616132853/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.918861 localstack-core-2.1.1.dev20230616132853/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.918861 localstack-core-2.1.1.dev20230616132853/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.918861 localstack-core-2.1.1.dev20230616132853/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43901 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.922861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.926861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.926861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.926861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.926861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.946861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.946861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.946861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.946861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.946861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.946861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.946861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.946861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.954861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.954861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.954861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.954861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.954861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.954861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.954861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.958861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.958861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.962861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.962861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.962861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.962861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.962861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.962861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.962861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.962861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.966861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.966861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.966861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.966861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.966861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.966861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.966861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.970861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4358 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2035 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4960 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4363 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3053 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4242 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3566 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.970861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.970861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.970861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.974861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.974861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1694 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.974861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.974861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3143 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.974861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5066 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.974861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.974861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.978861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.978861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31120 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.978861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.978861 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12321 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.978861 localstack-core-2.1.1.dev20230616132853/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.978861 localstack-core-2.1.1.dev20230616132853/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.978861 localstack-core-2.1.1.dev20230616132853/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.978861 localstack-core-2.1.1.dev20230616132853/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.982861 localstack-core-2.1.1.dev20230616132853/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.982861 localstack-core-2.1.1.dev20230616132853/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.982861 localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.986861 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69752 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.986861 localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.990861 localstack-core-2.1.1.dev20230616132853/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.990861 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.990861 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.990861 localstack-core-2.1.1.dev20230616132853/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.990861 localstack-core-2.1.1.dev20230616132853/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.990861 localstack-core-2.1.1.dev20230616132853/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.994861 localstack-core-2.1.1.dev20230616132853/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 13:29:01.994861 localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-16 13:29:01.000000 localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38094 2023-06-16 13:29:01.000000 localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 13:29:01.000000 localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-16 13:29:01.000000 localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 13:28:57.000000 localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-16 13:28:57.000000 localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-16 13:29:01.000000 localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-16 13:29:01.000000 localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-16 13:29:01.994861 localstack-core-2.1.1.dev20230616132853/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-16 12:55:17.000000 localstack-core-2.1.1.dev20230616132853/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230616121558/LICENSE.txt` & `localstack-core-2.1.1.dev20230616132853/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/Makefile` & `localstack-core-2.1.1.dev20230616132853/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/PKG-INFO` & `localstack-core-2.1.1.dev20230616132853/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230616121558
+Version: 2.1.1.dev20230616132853
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230616121558/README.md` & `localstack-core-2.1.1.dev20230616132853/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/bin/localstack` & `localstack-core-2.1.1.dev20230616132853/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230616132853/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230616132853/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230616132853/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230616132853/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230616132853/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230616132853/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230616132853/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/config.py` & `localstack-core-2.1.1.dev20230616132853/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/constants.py` & `localstack-core-2.1.1.dev20230616132853/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230616132853/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230616132853/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230616132853/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/client.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/request.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/response.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/http/router.py` & `localstack-core-2.1.1.dev20230616132853/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230616132853/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230616132853/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230616132853/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230616132853/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230616132853/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230616132853/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/packages/ffmpeg.py` & `localstack-core-2.1.1.dev20230616132853/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230616132853/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/plugins.py` & `localstack-core-2.1.1.dev20230616132853/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230616132853/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230616132853/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230616132853/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230616132853/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230616132853/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import copy
-from typing import Final
+from typing import Final, Optional
 
 from jsonpath_ng import parse
 
 from localstack.services.stepfunctions.asl.component.eval_component import EvalComponent
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 
 
 class ResultPath(EvalComponent):
     DEFAULT_PATH: Final[str] = "$"
 
     def __init__(self, result_path_src: str):
-        self.result_path_src: Final[str] = result_path_src
+        self.result_path_src: Final[Optional[str]] = result_path_src
 
     def _eval_body(self, env: Environment) -> None:
+        result = env.stack.pop()
+
+        if self.result_path_src is None:
+            return
+
         result_expr = parse(self.result_path_src)
-        result = copy.deepcopy(env.stack.pop())
         if env.inp is None:
             env.inp = dict()
-        env.inp = result_expr.update_or_create(env.inp, result)
+        env.inp = result_expr.update_or_create(env.inp, copy.deepcopy(result))
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,9 +15,16 @@
     @classmethod
     def from_raw(cls, string_dollar: str, string_path_context_obj: str):
         field: str = string_dollar[:-2]
         path_context_obj: str = string_path_context_obj[1:]
         return cls(field=field, path_context_obj=path_context_obj)
 
     def _eval_val(self, env: Environment) -> Any:
-        value = JSONPathUtils.extract_json(self.path_context_obj, env.context_object)
+        if self.path_context_obj.endswith("Task.Token"):
+            task_token = env.context_object_manager.update_task_token()
+            env.callback_pool_manager.add(task_token)
+            value = task_token
+        else:
+            value = JSONPathUtils.extract_json(
+                self.path_context_obj, env.context_object_manager.context_object
+            )
         return value
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         env.event_history.add_event(
             hist_type_event=self.state_entered_event_type,
             event_detail=EventDetails(
                 stateEnteredEventDetails=self._get_state_entered_even_details(env=env)
             ),
         )
 
-        env.context_object["State"] = State(
+        env.context_object_manager.context_object["State"] = State(
             EnteredTime=datetime.datetime.now().isoformat(), Name=self.name, RetryCount=0
         )
 
         # Filter the input onto the stack.
         if self.input_path:
             self.input_path.eval(env)
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,19 @@
         self.retry = state_props.get(RetryDecl)
         self.catch = state_props.get(CatchDecl)
 
         if not self.item_processor:
             raise ValueError(f"Missing ItemProcessor definition in props '{state_props}'.")
 
     def _eval_body(self, env: Environment) -> None:
-        env.context_object["Map"] = Map(Item=Item(Index=-1, Value="Unsupported"))
+        env.context_object_manager.context_object["Map"] = Map(
+            Item=Item(Index=-1, Value="Unsupported")
+        )
         super(StateMap, self)._eval_body(env=env)
-        env.context_object["Map"] = None
+        env.context_object_manager.context_object["Map"] = None
 
     def _eval_execution(self, env: Environment) -> None:
         # Reduce the input to the list of items.
         self.items_path.eval(env)
 
         # Launch the item processor.
         self.item_processor.eval(env)
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 
 
 # TODO: improve on factory constructor (don't use SubtypeManager)
 class StateTaskService(StateTask, abc.ABC):
     resource: ServiceResource
 
-    def _get_resource_type(self) -> str:
+    def _get_sfn_resource(self) -> str:
+        return self.resource.api_action
+
+    def _get_sfn_resource_type(self) -> str:
         return self.resource.service_name
 
     def _eval_parameters(self, env: Environment) -> dict:
         parameters = dict()
         if self.parameters:
             self.parameters.eval(env=env)
             env_parameters = env.stack.pop()
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,91 +1,57 @@
 from botocore.exceptions import ClientError
 
-from localstack.aws.api.stepfunctions import (
-    HistoryEventExecutionDataDetails,
-    HistoryEventType,
-    TaskFailedEventDetails,
-    TaskScheduledEventDetails,
-    TaskStartedEventDetails,
-    TaskSucceededEventDetails,
-)
+from localstack.aws.api.stepfunctions import HistoryEventType, TaskFailedEventDetails
 from localstack.aws.protocol.service_router import get_service_catalog
 from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
     FailureEvent,
 )
 from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name import (
     StatesErrorName,
 )
 from localstack.services.stepfunctions.asl.component.common.error_name.states_error_name_type import (
     StatesErrorNameType,
 )
-from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service import (
-    StateTaskService,
+from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service_callback import (
+    StateTaskServiceCallback,
 )
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
-from localstack.services.stepfunctions.asl.utils.encoding import to_json_str
 from localstack.utils.aws import aws_stack
 from localstack.utils.common import camel_to_snake_case
 
 
-class StateTaskServiceAwsSdk(StateTaskService):
-    def _get_resource_type(self) -> str:
-        return f"{self.resource.service_name}:{self.resource.api_name}"
-
-    def _eval_execution(self, env: Environment) -> None:
-        super()._eval_execution(env=env)
-
-        api_name = self.resource.api_name
-        api_action = camel_to_snake_case(self.resource.api_action)
-
-        parameters = self._eval_parameters(env=env)
+class StateTaskServiceAwsSdk(StateTaskServiceCallback):
+    _API_NAMES: dict[str, str] = {"sfn": "stepfunctions"}
+    _SFN_TO_BOTO_PARAM_NORMALISERS = {
+        "stepfunctions": {"send_task_success": {"Output": "output", "TaskToken": "taskToken"}}
+    }
 
-        # Simulate scheduled-start workflow.
-        parameters_str = to_json_str(parameters)
-        env.event_history.add_event(
-            hist_type_event=HistoryEventType.TaskScheduled,
-            event_detail=EventDetails(
-                taskScheduledEventDetails=TaskScheduledEventDetails(
-                    resourceType=self._get_resource_type(),
-                    resource=self.resource.api_action,
-                    region=self.resource.region,
-                    parameters=parameters_str,
-                )
-            ),
-        )
-        env.event_history.add_event(
-            hist_type_event=HistoryEventType.TaskStarted,
-            event_detail=EventDetails(
-                taskStartedEventDetails=TaskStartedEventDetails(
-                    resourceType=self._get_resource_type(),
-                    resource=self.resource.api_action,
-                )
-            ),
-        )
-
-        api_client = aws_stack.create_external_boto_client(service_name=api_name)
-
-        response = getattr(api_client, api_action)(**parameters) or dict()
-        if response:
-            response.pop("ResponseMetadata", None)
+    def _get_sfn_resource_type(self) -> str:
+        return f"{self.resource.service_name}:{self.resource.api_name}"
 
-        env.stack.append(response)
+    def _normalise_api_name(self, api_name: str) -> str:
+        return self._API_NAMES.get(api_name, api_name)
 
-        env.event_history.add_event(
-            hist_type_event=HistoryEventType.TaskSucceeded,
-            event_detail=EventDetails(
-                taskSucceededEventDetails=TaskSucceededEventDetails(
-                    resourceType=self._get_resource_type(),
-                    resource=self.resource.api_action,
-                    output=to_json_str(response),
-                    outputDetails=HistoryEventExecutionDataDetails(truncated=False),
-                )
-            ),
-        )
+    def _boto_normalise_parameters(self, api_name: str, api_action: str, parameters: dict) -> None:
+        api_normalisers = self._SFN_TO_BOTO_PARAM_NORMALISERS.get(api_name)
+        if not api_normalisers:
+            return
+
+        action_normalisers = api_normalisers.get(api_action)
+        if not action_normalisers:
+            return None
+
+        parameter_keys = list(parameters.keys())
+        for parameter_key in parameter_keys:
+            norm_parameter_key = action_normalisers.get(parameter_key)
+            if norm_parameter_key:
+                tmp = parameters[parameter_key]
+                del parameters[parameter_key]
+                parameters[norm_parameter_key] = tmp
 
     @staticmethod
     def _normalise_service_name(service_name: str) -> str:
         return get_service_catalog().get(service_name).service_id.replace(" ", "")
 
     @staticmethod
     def _normalise_exception_name(norm_service_name: str, ex: Exception) -> str:
@@ -94,16 +60,16 @@
 
     def _get_task_failure_event(self, error: str, cause: str) -> FailureEvent:
         return FailureEvent(
             error_name=StatesErrorName(typ=StatesErrorNameType.StatesTaskFailed),
             event_type=HistoryEventType.TaskFailed,
             event_details=EventDetails(
                 taskFailedEventDetails=TaskFailedEventDetails(
-                    resourceType=self._get_resource_type(),
-                    resource=self.resource.api_action,
+                    resource=self._get_sfn_resource(),
+                    resourceType=self._get_sfn_resource_type(),
                     error=error,
                     cause=cause,
                 )
             ),
         )
 
     def _from_error(self, env: Environment, ex: Exception) -> FailureEvent:
@@ -125,7 +91,24 @@
             failure_event = self._get_task_failure_event(error=error, cause=cause)
             return failure_event
 
         failure_event = self._get_task_failure_event(
             error=error, cause=str(ex)  # TODO: update cause decoration.
         )
         return failure_event
+
+    def _eval_service_task(self, env: Environment, parameters: dict) -> None:
+        api_name = self.resource.api_name
+        api_name = self._normalise_api_name(api_name)
+        api_action = camel_to_snake_case(self.resource.api_action)
+
+        self._boto_normalise_parameters(
+            api_name=api_name, api_action=api_action, parameters=parameters
+        )
+
+        api_client = aws_stack.create_external_boto_client(service_name=api_name)
+
+        response = getattr(api_client, api_action)(**parameters) or dict()
+        if response:
+            response.pop("ResponseMetadata", None)
+
+        env.stack.append(response)
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,133 +1,105 @@
-from typing import Final, Optional
-
-from botocore.exceptions import ClientError
+import json
+from abc import abstractmethod
 
 from localstack.aws.api.stepfunctions import (
     HistoryEventExecutionDataDetails,
     HistoryEventType,
-    TaskFailedEventDetails,
     TaskScheduledEventDetails,
     TaskStartedEventDetails,
+    TaskSubmittedEventDetails,
     TaskSucceededEventDetails,
 )
-from localstack.services.stepfunctions.asl.component.common.error_name.custom_error_name import (
-    CustomErrorName,
-)
-from localstack.services.stepfunctions.asl.component.common.error_name.failure_event import (
-    FailureEvent,
+from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.resource import (
+    ResourceCondition,
 )
 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.state_task_service import (
     StateTaskService,
 )
+from localstack.services.stepfunctions.asl.eval.callback.callback import CallbackOutcomeSuccess
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 from localstack.services.stepfunctions.asl.eval.event.event_detail import EventDetails
 from localstack.services.stepfunctions.asl.utils.encoding import to_json_str
-from localstack.utils.aws import aws_stack
-from localstack.utils.strings import camel_to_snake_case
 
 
-class StateTaskServiceSqs(StateTaskService):
-    _ERROR_NAME_CLIENT: Final[str] = "SQS.SdkClientException"
-    _ERROR_NAME_AWS: Final[str] = "SQS.AmazonSQSException"
-
-    _SUPPORTED_API_PARAM_BINDINGS: Final[dict[str, set[str]]] = {
-        "sendmessage": {
-            "DelaySeconds",
-            "MessageAttribute",
-            "MessageBody",
-            "MessageDeduplicationId",
-            "MessageGroupId",
-            "QueueUrl",
-        }
-    }
-
-    def _from_error(self, env: Environment, ex: Exception) -> FailureEvent:
-        if isinstance(ex, ClientError):
-            return FailureEvent(
-                error_name=CustomErrorName(self._ERROR_NAME_CLIENT),
-                event_type=HistoryEventType.TaskFailed,
-                event_details=EventDetails(
-                    taskFailedEventDetails=TaskFailedEventDetails(
-                        error=self._ERROR_NAME_CLIENT,
-                        cause=ex.response["Error"][
-                            "Message"
-                        ],  # TODO: update to report expected cause.
-                        resource=self.resource.api_action,
-                        resourceType=self.resource.service_name,
-                    )
-                ),
-            )
+class StateTaskServiceCallback(StateTaskService):
+    def _get_sfn_resource(self) -> str:
+        resource = super()._get_sfn_resource()
+        if self.resource.condition is not None:
+            resource += f".{self.resource.condition}"
+        return resource
+
+    @abstractmethod
+    def _eval_service_task(self, env: Environment, parameters: dict):
+        ...
+
+    def _wait_for_task_token(self, env: Environment) -> None:  # noqa
+        callback_id = env.context_object_manager.context_object["Task"]["Token"]
+        callback_endpoint = env.callback_pool_manager.get(callback_id)
+        outcome = callback_endpoint.wait()  # TODO: implement timeout.
+
+        if isinstance(outcome, CallbackOutcomeSuccess):
+            outcome_output = json.loads(outcome.output)
+            env.stack.append(outcome_output)
         else:
-            return FailureEvent(
-                error_name=CustomErrorName(self._ERROR_NAME_AWS),
-                event_type=HistoryEventType.TaskFailed,
-                event_details=EventDetails(
-                    taskFailedEventDetails=TaskFailedEventDetails(
-                        error=self._ERROR_NAME_AWS,
-                        cause=str(ex),  # TODO: update to report expected cause.
-                        resource=self.resource.api_action,
-                        resourceType=self.resource.service_name,
-                    )
-                ),
-            )
+            raise NotImplementedError(f"Unsupported Callbackoutcome type '{type(outcome)}'.")
 
-    def _eval_parameters(self, env: Environment) -> dict:
-        api_action: str = self.resource.api_action
-        supported_parameters: Optional[set[str]] = self._SUPPORTED_API_PARAM_BINDINGS.get(
-            api_action.lower(), None
-        )
-        if supported_parameters is None:
-            raise RuntimeError("TODO: raise unsupported api error?")
-
-        parameters: dict = super()._eval_parameters(env=env)
-        unsupported_parameters: list[str] = [
-            parameter for parameter in parameters.keys() if parameter not in supported_parameters
-        ]
-        if unsupported_parameters:
-            for unsupported_parameter in unsupported_parameters:
-                parameters.pop(unsupported_parameter, None)
-
-        return parameters
+    def _is_condition(self):
+        return self.resource.condition is not None
 
     def _eval_execution(self, env: Environment) -> None:
         parameters = self._eval_parameters(env=env)
-
         parameters_str = to_json_str(parameters)
+
         env.event_history.add_event(
             hist_type_event=HistoryEventType.TaskScheduled,
             event_detail=EventDetails(
                 taskScheduledEventDetails=TaskScheduledEventDetails(
-                    resourceType=self._get_resource_type(),
-                    resource=self.resource.api_action,
+                    resource=self._get_sfn_resource(),
+                    resourceType=self._get_sfn_resource_type(),
                     region=self.resource.region,
                     parameters=parameters_str,
                 )
             ),
         )
         env.event_history.add_event(
             hist_type_event=HistoryEventType.TaskStarted,
             event_detail=EventDetails(
                 taskStartedEventDetails=TaskStartedEventDetails(
-                    resourceType=self._get_resource_type(),
-                    resource=self.resource.api_action,
+                    resource=self._get_sfn_resource(), resourceType=self._get_sfn_resource_type()
                 )
             ),
         )
 
-        api_action = camel_to_snake_case(self.resource.api_action)
-        sqs_client = aws_stack.create_external_boto_client("sqs")
-        response = getattr(sqs_client, api_action)(**parameters)
-        response.pop("ResponseMetadata", None)
-        env.stack.append(response)
+        self._eval_service_task(env=env, parameters=parameters)
+
+        if self._is_condition():
+            output = env.stack.pop()
+            env.event_history.add_event(
+                hist_type_event=HistoryEventType.TaskSubmitted,
+                event_detail=EventDetails(
+                    taskSubmittedEventDetails=TaskSubmittedEventDetails(
+                        resource=self._get_sfn_resource(),
+                        resourceType=self._get_sfn_resource_type(),
+                        output=to_json_str(output),
+                        outputDetails=HistoryEventExecutionDataDetails(truncated=False),
+                    )
+                ),
+            )
+            match self.resource.condition:
+                case ResourceCondition.WaitForTaskToken:
+                    self._wait_for_task_token(env=env)
+                case unsupported:
+                    raise NotImplementedError(f"Unsupported callback type '{unsupported}'.")
 
+        output = env.stack[-1]
         env.event_history.add_event(
             hist_type_event=HistoryEventType.TaskSucceeded,
             event_detail=EventDetails(
                 taskSucceededEventDetails=TaskSucceededEventDetails(
-                    resourceType=self._get_resource_type(),
-                    resource=self.resource.api_action,
-                    output=to_json_str(response),
+                    resource=self._get_sfn_resource(),
+                    resourceType=self._get_sfn_resource_type(),
+                    output=to_json_str(output),
                     outputDetails=HistoryEventExecutionDataDetails(truncated=False),
                 )
             ),
         )
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from localstack.services.stepfunctions.asl.component.state.state_execution.execute_state import (
     ExecutionState,
 )
 from localstack.services.stepfunctions.asl.component.state.state_execution.state_task.service.resource import (
     Resource,
 )
 from localstack.services.stepfunctions.asl.component.state.state_props import StateProps
-from localstack.services.stepfunctions.asl.eval.contextobject.contex_object import Task
 from localstack.services.stepfunctions.asl.eval.environment import Environment
 
 
 class StateTask(ExecutionState, abc.ABC):
     resource: Resource
 
     def __init__(self):
@@ -57,10 +56,11 @@
 
     def from_state_props(self, state_props: StateProps) -> None:
         super(StateTask, self).from_state_props(state_props)
         self.parameters = state_props.get(Parameters)
         self.resource = state_props.get(Resource)
 
     def _eval_body(self, env: Environment) -> None:
-        env.context_object["Task"] = Task(Token="Unsupported")
+        if self.name == "Send":
+            print(self.name)
         super(StateTask, self)._eval_body(env=env)
-        env.context_object["Task"] = None
+        env.context_object_manager.context_object["Task"] = None
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 
     def from_state_props(self, state_props: StateProps) -> None:
         super(StatePass, self).from_state_props(state_props)
         self.result = state_props.get(Result)
         self.result_path = state_props.get(ResultPath)
         self.parameters = state_props.get(Parameters)
 
-        if self.result is not None and self.result_path is None:
+        if self.result_path is None:
             self.result_path = ResultPath(result_path_src=ResultPath.DEFAULT_PATH)
 
     def _eval_state(self, env: Environment) -> None:
+        if self.name == "ParseBody":
+            print(self.name)
+
         if self.parameters:
             self.parameters.eval(env=env)
-            env.inp = env.stack.pop()
 
         if self.result:
             env.stack.append(self.result.result_obj)
-        else:
-            env.stack.append(env.inp)
 
         if self.result_path:
             self.result_path.eval(env)
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             return
         elif isinstance(env.program_state(), ProgramRunning):
             # Unrelated interrupt: continue waiting.
             LOG.info(
                 f"Wait function '{self}' successfully reentered waiting for "
                 f"another '{max_seconds - tot_sec_waited}' seconds."
             )
-            return WaitFunction._wait_interval(
+            return self._wait_interval(
                 env=env, seconds_waited=tot_sec_waited, max_seconds=max_seconds
             )
         else:
             LOG.info(
                 f"Wait function '{self}' successfully interrupted after '{tot_sec_waited}' seconds."
             )
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 import copy
 import logging
 import threading
 from typing import Any, Optional
 
 from localstack.aws.api.stepfunctions import ExecutionFailedEventDetails, Timestamp
+from localstack.services.stepfunctions.asl.eval.callback.callback import CallbackPoolManager
 from localstack.services.stepfunctions.asl.eval.contextobject.contex_object import (
     ContextObject,
     ContextObjectInitData,
+    ContextObjectManager,
 )
 from localstack.services.stepfunctions.asl.eval.event.event_history import EventHistory
 from localstack.services.stepfunctions.asl.eval.programstate.program_ended import ProgramEnded
 from localstack.services.stepfunctions.asl.eval.programstate.program_error import ProgramError
 from localstack.services.stepfunctions.asl.eval.programstate.program_running import ProgramRunning
 from localstack.services.stepfunctions.asl.eval.programstate.program_state import ProgramState
 from localstack.services.stepfunctions.asl.eval.programstate.program_stopped import ProgramStopped
@@ -25,37 +27,40 @@
         super(Environment, self).__init__()
         self._state_mutex = threading.RLock()
         self._program_state: Optional[ProgramState] = None
         self.program_state_event = threading.Event()
         self._frames: list[Environment] = list()
 
         self.event_history: EventHistory = EventHistory()
+        self.callback_pool_manager: CallbackPoolManager = CallbackPoolManager()
 
         self.heap: dict[str, Any] = dict()
         self.stack: list[Any] = list()
         self.inp: Optional[Any] = None
 
-        self.context_object: ContextObject = ContextObject(
-            Execution=context_object_init["Execution"],
-            StateMachine=context_object_init["StateMachine"],
-            State=None,
-            Task=None,
-            Map=None,
+        self.context_object_manager: ContextObjectManager = ContextObjectManager(
+            context_object=ContextObject(
+                Execution=context_object_init["Execution"],
+                StateMachine=context_object_init["StateMachine"],
+                State=None,
+                Task=None,
+                Map=None,
+            )
         )
 
     @classmethod
     def as_frame_of(cls, env: Environment):
         context_object_init = ContextObjectInitData(
-            Execution=env.context_object["Execution"],
-            StateMachine=env.context_object["StateMachine"],
+            Execution=env.context_object_manager.context_object["Execution"],
+            StateMachine=env.context_object_manager.context_object["StateMachine"],
         )
         frame = cls(context_object_init=context_object_init)
         frame.heap = env.heap
         frame.event_history = env.event_history
-        frame.context_object = env.context_object
+        frame.context_object = env.context_object_manager.context_object
         return frame
 
     @property
     def next_state_name(self) -> Optional[str]:
         next_state_name: Optional[str] = None
         if isinstance(self._program_state, ProgramRunning):
             next_state_name = self._program_state.next_state_name
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,16 @@
 from localstack.services.stepfunctions.asl.component.states import States
 from localstack.services.stepfunctions.asl.parse.typed_props import TypedProps
 
 
 class Preprocessor(ASLParserVisitor):
     @staticmethod
     def _inner_string_of(parse_tree: ParseTree) -> Optional[str]:
+        if Antlr4Utils.is_terminal(parse_tree, ASLLexer.NULL):
+            return None
         pt = Antlr4Utils.is_production(parse_tree) or Antlr4Utils.is_terminal(parse_tree)
         inner_str = pt.getText()
         if inner_str.startswith('"') and inner_str.endswith('"'):
             inner_str = inner_str[1:-1]
         return inner_str
 
     def visitComment_decl(self, ctx: ASLParser.Comment_declContext) -> Comment:
@@ -233,15 +235,15 @@
         return End(is_end=is_end)
 
     def visitNext_decl(self, ctx: ASLParser.Next_declContext) -> Next:
         inner_str = self._inner_string_of(parse_tree=ctx.keyword_or_string())
         return Next(name=inner_str)
 
     def visitResult_path_decl(self, ctx: ASLParser.Result_path_declContext) -> ResultPath:
-        inner_str = self._inner_string_of(parse_tree=ctx.keyword_or_string())
+        inner_str = self._inner_string_of(parse_tree=ctx.children[-1])
         return ResultPath(result_path_src=inner_str)
 
     def visitInput_path_decl(self, ctx: ASLParser.Input_path_declContext) -> InputPath:
         inner_str = self._inner_string_of(parse_tree=ctx.keyword_or_string())
         return InputPath(input_path_src=inner_str)
 
     def visitOutput_path_decl(self, ctx: ASLParser.Output_path_declContext):
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/provider_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,35 +12,46 @@
     DescribeStateMachineOutput,
     ExecutionList,
     ExecutionStatus,
     GetExecutionHistoryOutput,
     IncludeExecutionDataGetExecutionHistory,
     InvalidExecutionInput,
     InvalidName,
+    InvalidToken,
     ListExecutionsOutput,
     ListExecutionsPageToken,
     ListStateMachinesOutput,
     LongArn,
     Name,
     PageSize,
     PageToken,
     ReverseOrder,
+    SendTaskFailureOutput,
+    SendTaskSuccessOutput,
     SensitiveCause,
     SensitiveData,
     SensitiveError,
     StartExecutionOutput,
     StateMachineAlreadyExists,
     StateMachineDoesNotExist,
     StateMachineList,
     StateMachineStatus,
     StateMachineType,
     StepfunctionsApi,
     StopExecutionOutput,
+    TaskDoesNotExist,
+    TaskTimedOut,
+    TaskToken,
     TraceHeader,
 )
+from localstack.services.stepfunctions.asl.eval.callback.callback import (
+    CallbackConsumerTimeout,
+    CallbackNotifyConsumerError,
+    CallbackOutcomeSuccess,
+)
 from localstack.services.stepfunctions.backend.execution import Execution
 from localstack.services.stepfunctions.backend.state_machine import StateMachine
 from localstack.services.stepfunctions.backend.store import SFNStore, sfn_stores
 from localstack.utils.aws.arns import ArnData, parse_arn
 from localstack.utils.aws.arns import state_machine_arn as aws_stack_state_machine_arn
 from localstack.utils.strings import long_uid
 
@@ -143,14 +154,54 @@
             definition=sm.definition,
             roleArn=sm.role_arn,
             type=sm.sm_type,
             creationDate=sm.create_date,
             loggingConfiguration=sm.logging_config,
         )
 
+    def send_task_success(
+        self, context: RequestContext, task_token: TaskToken, output: SensitiveData
+    ) -> SendTaskSuccessOutput:
+        outcome = CallbackOutcomeSuccess(callback_id=task_token, output=output)
+        store = self.get_store(context)
+        for exec in store.executions.values():
+            try:
+                if exec.exec_worker.env.callback_pool_manager.notify(
+                    callback_id=task_token, outcome=outcome
+                ):
+                    return SendTaskSuccessOutput()
+            except CallbackNotifyConsumerError as consumer_error:
+                if isinstance(consumer_error, CallbackConsumerTimeout):
+                    raise TaskTimedOut()
+                else:
+                    raise TaskDoesNotExist()
+        raise InvalidToken()
+
+    def send_task_failure(
+        self,
+        context: RequestContext,
+        task_token: TaskToken,
+        error: SensitiveError = None,
+        cause: SensitiveCause = None,
+    ) -> SendTaskFailureOutput:
+        outcome = CallbackOutcomeSuccess(callback_id=task_token)
+        store = self.get_store(context)
+        for exec in store.executions.values():
+            try:
+                if exec.exec_worker.env.callback_pool_manager.notify(
+                    callback_id=task_token, outcome=outcome
+                ):
+                    return SendTaskFailureOutput()
+            except CallbackNotifyConsumerError as consumer_error:
+                if isinstance(consumer_error, CallbackConsumerTimeout):
+                    raise TaskTimedOut()
+                else:
+                    raise TaskDoesNotExist()
+        raise InvalidToken()
+
     def start_execution(
         self,
         context: RequestContext,
         state_machine_arn: Arn,
         name: Name = None,
         input: SensitiveData = None,
         trace_header: TraceHeader = None,
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230616132853/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/state/core.py` & `localstack-core-2.1.1.dev20230616132853/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230616132853/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230616132853/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230616132853/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230616132853/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/collections.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230616132853/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230616121558
+Version: 2.1.1.dev20230616132853
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -522,14 +522,15 @@
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
 localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
 localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
 localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
 localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
 localstack/services/stepfunctions/asl/component/state/state_pass/result.py
 localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
@@ -544,14 +545,16 @@
 localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
 localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
 localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
 localstack/services/stepfunctions/asl/eval/__init__.py
 localstack/services/stepfunctions/asl/eval/count_down_latch.py
 localstack/services/stepfunctions/asl/eval/environment.py
 localstack/services/stepfunctions/asl/eval/program_worker.py
+localstack/services/stepfunctions/asl/eval/callback/__init__.py
+localstack/services/stepfunctions/asl/eval/callback/callback.py
 localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
 localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
 localstack/services/stepfunctions/asl/eval/event/__init__.py
 localstack/services/stepfunctions/asl/eval/event/event_detail.py
 localstack/services/stepfunctions/asl/eval/event/event_history.py
 localstack/services/stepfunctions/asl/eval/programstate/__init__.py
 localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8937908496732025%*

 * *Differences: {"'localstack.hooks.on_infra_ready'": '{insert: [(1, '*

 * *                                      "'register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes')], "*

 * *                                      'delete: [0]}',*

 * * "'localstack.hooks.on_infra_start'": '{insert: [(4, '*

 * *                                      "'validate_configuration=localstack.services.awslambda.plugins:validate_configuration'), "*

 * *                                      '(5, '*

 * *                                   […]*

```diff
@@ -45,44 +45,44 @@
         "swf:default=localstack.services.providers:swf",
         "transcribe:default=localstack.services.providers:transcribe"
     ],
     "localstack.hooks.configure_localstack_container": [
         "configure_edge_port=localstack.plugins:configure_edge_port"
     ],
     "localstack.hooks.on_infra_ready": [
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
     ],
     "localstack.hooks.on_infra_shutdown": [
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
         "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
     ],
     "localstack.hooks.on_infra_start": [
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
         "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
         "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
-        "terraform/community=localstack.packages.plugins:terraform_package"
+        "terraform/community=localstack.packages.plugins:terraform_package",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230616121558/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230616132853/localstack_core.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 pypandoc
 pyproject-flake8>=6.0.0.post1
 rstr>=3.2.0
 
 [full]
 airspeed-ext==0.5.19
 amazon_kclpy!=2.1.0,>=2.0.6
-antlr4-python3-runtime==4.11.1
+antlr4-python3-runtime==4.12.0
 apispec>=5.1.1
 aws-sam-translator>=1.15.1
 awscli>=1.22.90
 awscrt>=0.13.14
 boto>=2.49.0
 boto3>=1.26.121
 botocore>=1.29.133
@@ -70,15 +70,15 @@
 vosk==0.3.43
 Werkzeug>=2.3.4
 xmltodict>=0.11.0
 
 [runtime]
 airspeed-ext==0.5.19
 amazon_kclpy!=2.1.0,>=2.0.6
-antlr4-python3-runtime==4.11.1
+antlr4-python3-runtime==4.12.0
 apispec>=5.1.1
 aws-sam-translator>=1.15.1
 awscli>=1.22.90
 awscrt>=0.13.14
 boto>=2.49.0
 boto3>=1.26.121
 botocore>=1.29.133
```

### Comparing `localstack-core-2.1.1.dev20230616121558/pyproject.toml` & `localstack-core-2.1.1.dev20230616132853/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230616121558/setup.cfg` & `localstack-core-2.1.1.dev20230616132853/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 	services/**/*.html
 	utils/kinesis/java/cloud/localstack/*.*
 
 [options.extras_require]
 runtime = 
 	airspeed-ext==0.5.19
 	amazon_kclpy>=2.0.6,!=2.1.0
-	antlr4-python3-runtime==4.11.1
+	antlr4-python3-runtime==4.12.0
 	apispec>=5.1.1
 	aws-sam-translator>=1.15.1
 	awscli>=1.22.90
 	awscrt>=0.13.14
 	boto>=2.49.0
 	boto3>=1.26.121
 	botocore>=1.29.133
```

