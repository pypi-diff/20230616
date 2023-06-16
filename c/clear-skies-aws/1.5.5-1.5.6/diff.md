# Comparing `tmp/clear_skies_aws-1.5.5.tar.gz` & `tmp/clear_skies_aws-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_aws-1.5.5.tar", max compression
+gzip compressed data, was "clear_skies_aws-1.5.6.tar", max compression
```

## Comparing `clear_skies_aws-1.5.5.tar` & `clear_skies_aws-1.5.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1053 2022-01-16 00:26:29.571128 clear_skies_aws-1.5.5/LICENSE
--rw-r--r--   0        0        0     7780 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.5/README.md
--rw-r--r--   0        0        0      789 2023-06-08 15:29:09.129232 clear_skies_aws-1.5.5/pyproject.toml
--rw-r--r--   0        0        0       58 2023-05-23 15:29:15.831933 clear_skies_aws-1.5.5/src/clearskies_aws/__init__.py
--rw-r--r--   0        0        0     2141 2023-06-07 12:04:20.019789 clear_skies_aws-1.5.5/src/clearskies_aws/actions/__init__.py
--rw-r--r--   0        0        0     3357 2023-06-08 12:35:36.805017 clear_skies_aws-1.5.5/src/clearskies_aws/actions/action_aws.py
--rw-r--r--   0        0        0     4085 2023-06-07 00:11:48.817084 clear_skies_aws-1.5.5/src/clearskies_aws/actions/assume_role.py
--rw-r--r--   0        0        0     2450 2023-06-07 00:11:48.873084 clear_skies_aws-1.5.5/src/clearskies_aws/actions/assume_role_test.py
--rw-r--r--   0        0        0     6914 2023-06-08 12:07:05.650182 clear_skies_aws-1.5.5/src/clearskies_aws/actions/ses.py
--rw-r--r--   0        0        0     1630 2023-06-07 12:04:20.019789 clear_skies_aws-1.5.5/src/clearskies_aws/actions/ses_test.py
--rw-r--r--   0        0        0     2197 2023-06-08 12:06:42.106108 clear_skies_aws-1.5.5/src/clearskies_aws/actions/sns.py
--rw-r--r--   0        0        0     2194 2023-06-07 19:38:57.987774 clear_skies_aws-1.5.5/src/clearskies_aws/actions/sns_test.py
--rw-r--r--   0        0        0     2340 2023-06-08 12:07:13.458206 clear_skies_aws-1.5.5/src/clearskies_aws/actions/sqs.py
--rw-r--r--   0        0        0     2234 2023-06-06 22:38:31.426673 clear_skies_aws-1.5.5/src/clearskies_aws/actions/sqs_test.py
--rw-r--r--   0        0        0       83 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.5/src/clearskies_aws/backends/__init__.py
--rw-r--r--   0        0        0    29126 2023-05-17 10:18:33.296047 clear_skies_aws-1.5.5/src/clearskies_aws/backends/dynamo_db_backend.py
--rw-r--r--   0        0        0    13150 2023-04-27 10:33:09.319573 clear_skies_aws-1.5.5/src/clearskies_aws/backends/dynamo_db_backend_test.py
--rw-r--r--   0        0        0     2726 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.5/src/clearskies_aws/backends/sqs_backend.py
--rw-r--r--   0        0        0     1138 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.5/src/clearskies_aws/backends/sqs_backend_test.py
--rw-r--r--   0        0        0      324 2023-06-07 19:43:15.680620 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/__init__.py
--rw-r--r--   0        0        0     1305 2023-03-26 13:26:58.707778 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1276 2023-03-26 13:26:58.707778 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1251 2023-03-26 13:26:58.707778 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0      506 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/cli.py
--rw-r--r--   0        0        0     1002 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_api_gateway.py
--rw-r--r--   0        0        0      952 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_elb.py
--rw-r--r--   0        0        0     1009 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_http_gateway.py
--rw-r--r--   0        0        0     1183 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_invocation.py
--rw-r--r--   0        0        0     1333 2023-06-08 15:28:34.556614 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_sns.py
--rw-r--r--   0        0        0     1678 2023-04-04 23:13:02.122630 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
--rw-r--r--   0        0        0     1999 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
--rw-r--r--   0        0        0       56 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.5/src/clearskies_aws/di/__init__.py
--rw-r--r--   0        0        0      775 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.5/src/clearskies_aws/di/standard_dependencies.py
--rw-r--r--   0        0        0      267 2023-06-07 19:44:19.148834 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/__init__.py
--rw-r--r--   0        0        0      943 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     3710 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     2761 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
--rw-r--r--   0        0        0      901 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0     2932 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_api_gateway.py
--rw-r--r--   0        0        0     2845 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
--rw-r--r--   0        0        0      662 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_elb.py
--rw-r--r--   0        0        0      692 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_http_gateway.py
--rw-r--r--   0        0        0      715 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_invocation.py
--rw-r--r--   0        0        0     2211 2023-06-08 15:28:43.616775 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_sns.py
--rw-r--r--   0        0        0     2047 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
--rw-r--r--   0        0        0       22 2023-05-23 15:29:05.208303 clear_skies_aws-1.5.5/src/clearskies_aws/mocks/__init__.py
--rw-r--r--   0        0        0       21 2023-05-23 15:29:05.208303 clear_skies_aws-1.5.5/src/clearskies_aws/mocks/actions/__init__.py
--rw-r--r--   0        0        0      911 2023-05-23 15:29:05.208303 clear_skies_aws-1.5.5/src/clearskies_aws/mocks/actions/ses.py
--rw-r--r--   0        0        0      121 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/__init__.py
--rw-r--r--   0        0        0     1919 2023-05-19 13:30:13.392139 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/__init__.py
--rw-r--r--   0        0        0     1082 2023-03-26 13:26:58.719778 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
--rw-r--r--   0        0        0     3467 2023-05-19 13:34:03.783513 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
--rw-r--r--   0        0        0     3776 2023-03-26 13:26:58.719778 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
--rw-r--r--   0        0        0     6444 2023-03-26 13:26:58.719778 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
--rw-r--r--   0        0        0     1655 2023-04-14 14:57:45.726909 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/parameter_store.py
--rw-r--r--   0        0        0      761 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/parameter_store_test.py
--rw-r--r--   0        0        0     2898 2023-04-14 14:57:45.758909 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/secrets_manager.py
--rw-r--r--   0        0        0      786 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.5/src/clearskies_aws/secrets/secrets_manager_test.py
--rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1053 2022-01-16 00:26:29.571128 clear_skies_aws-1.5.6/LICENSE
+-rw-r--r--   0        0        0     7780 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.6/README.md
+-rw-r--r--   0        0        0      789 2023-06-16 01:37:13.694854 clear_skies_aws-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-05-23 15:29:15.831933 clear_skies_aws-1.5.6/src/clearskies_aws/__init__.py
+-rw-r--r--   0        0        0     2141 2023-06-07 12:04:20.019789 clear_skies_aws-1.5.6/src/clearskies_aws/actions/__init__.py
+-rw-r--r--   0        0        0     3357 2023-06-08 12:35:36.805017 clear_skies_aws-1.5.6/src/clearskies_aws/actions/action_aws.py
+-rw-r--r--   0        0        0     4085 2023-06-07 00:11:48.817084 clear_skies_aws-1.5.6/src/clearskies_aws/actions/assume_role.py
+-rw-r--r--   0        0        0     2450 2023-06-07 00:11:48.873084 clear_skies_aws-1.5.6/src/clearskies_aws/actions/assume_role_test.py
+-rw-r--r--   0        0        0     6914 2023-06-08 12:07:05.650182 clear_skies_aws-1.5.6/src/clearskies_aws/actions/ses.py
+-rw-r--r--   0        0        0     1630 2023-06-07 12:04:20.019789 clear_skies_aws-1.5.6/src/clearskies_aws/actions/ses_test.py
+-rw-r--r--   0        0        0     2197 2023-06-08 12:06:42.106108 clear_skies_aws-1.5.6/src/clearskies_aws/actions/sns.py
+-rw-r--r--   0        0        0     2194 2023-06-07 19:38:57.987774 clear_skies_aws-1.5.6/src/clearskies_aws/actions/sns_test.py
+-rw-r--r--   0        0        0     2340 2023-06-08 12:07:13.458206 clear_skies_aws-1.5.6/src/clearskies_aws/actions/sqs.py
+-rw-r--r--   0        0        0     2234 2023-06-06 22:38:31.426673 clear_skies_aws-1.5.6/src/clearskies_aws/actions/sqs_test.py
+-rw-r--r--   0        0        0       83 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.6/src/clearskies_aws/backends/__init__.py
+-rw-r--r--   0        0        0    29126 2023-05-17 10:18:33.296047 clear_skies_aws-1.5.6/src/clearskies_aws/backends/dynamo_db_backend.py
+-rw-r--r--   0        0        0    13150 2023-04-27 10:33:09.319573 clear_skies_aws-1.5.6/src/clearskies_aws/backends/dynamo_db_backend_test.py
+-rw-r--r--   0        0        0     2726 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.6/src/clearskies_aws/backends/sqs_backend.py
+-rw-r--r--   0        0        0     1138 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.6/src/clearskies_aws/backends/sqs_backend_test.py
+-rw-r--r--   0        0        0      325 2023-06-16 01:31:49.897322 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/__init__.py
+-rw-r--r--   0        0        0     1305 2023-03-26 13:26:58.707778 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1276 2023-03-26 13:26:58.707778 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1251 2023-03-26 13:26:58.707778 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0      506 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/cli.py
+-rw-r--r--   0        0        0     1002 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_api_gateway.py
+-rw-r--r--   0        0        0      952 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_elb.py
+-rw-r--r--   0        0        0     1009 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_http_gateway.py
+-rw-r--r--   0        0        0     1183 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_invocation.py
+-rw-r--r--   0        0        0     1342 2023-06-16 01:36:04.338530 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_sns.py
+-rw-r--r--   0        0        0     1678 2023-04-04 23:13:02.122630 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
+-rw-r--r--   0        0        0     1999 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
+-rw-r--r--   0        0        0       56 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.6/src/clearskies_aws/di/__init__.py
+-rw-r--r--   0        0        0      775 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.6/src/clearskies_aws/di/standard_dependencies.py
+-rw-r--r--   0        0        0      267 2023-06-07 19:44:19.148834 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/__init__.py
+-rw-r--r--   0        0        0      943 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     3710 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     2761 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
+-rw-r--r--   0        0        0      901 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0     2932 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_api_gateway.py
+-rw-r--r--   0        0        0     2845 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
+-rw-r--r--   0        0        0      662 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_elb.py
+-rw-r--r--   0        0        0      692 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_http_gateway.py
+-rw-r--r--   0        0        0      715 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_invocation.py
+-rw-r--r--   0        0        0     2081 2023-06-16 01:36:39.962697 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_sns.py
+-rw-r--r--   0        0        0     2047 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
+-rw-r--r--   0        0        0       22 2023-05-23 15:29:05.208303 clear_skies_aws-1.5.6/src/clearskies_aws/mocks/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-23 15:29:05.208303 clear_skies_aws-1.5.6/src/clearskies_aws/mocks/actions/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-23 15:29:05.208303 clear_skies_aws-1.5.6/src/clearskies_aws/mocks/actions/ses.py
+-rw-r--r--   0        0        0      121 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/__init__.py
+-rw-r--r--   0        0        0     1919 2023-05-19 13:30:13.392139 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/__init__.py
+-rw-r--r--   0        0        0     1082 2023-03-26 13:26:58.719778 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
+-rw-r--r--   0        0        0     3467 2023-05-19 13:34:03.783513 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
+-rw-r--r--   0        0        0     3776 2023-03-26 13:26:58.719778 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
+-rw-r--r--   0        0        0     6444 2023-03-26 13:26:58.719778 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
+-rw-r--r--   0        0        0     1655 2023-04-14 14:57:45.726909 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/parameter_store.py
+-rw-r--r--   0        0        0      761 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/parameter_store_test.py
+-rw-r--r--   0        0        0     2898 2023-04-14 14:57:45.758909 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/secrets_manager.py
+-rw-r--r--   0        0        0      786 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.6/src/clearskies_aws/secrets/secrets_manager_test.py
+-rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.5.6/PKG-INFO
```

### Comparing `clear_skies_aws-1.5.5/LICENSE` & `clear_skies_aws-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/README.md` & `clear_skies_aws-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/pyproject.toml` & `clear_skies_aws-1.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-aws"
-version = "1.5.5"
+version = "1.5.6"
 description = "clearskies bindings for working in AWS"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
     "tnijboer"
 ]
 repository = "https://github.com/cmancone/clearskies-aws"
 license = "MIT"
```

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/__init__.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/action_aws.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/action_aws.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/assume_role.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/assume_role.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/assume_role_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/assume_role_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/ses.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/ses_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/ses_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/sns.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/sns_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/sns_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/sqs.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/sqs.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/actions/sqs_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/actions/sqs_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/backends/dynamo_db_backend.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/backends/dynamo_db_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/backends/dynamo_db_backend_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/backends/dynamo_db_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/backends/sqs_backend.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/backends/sqs_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/backends/sqs_backend_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/backends/sqs_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_api_gateway.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_elb.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_http_gateway.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_invocation.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_sns.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_sns.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,27 +17,27 @@
     def __call__(self, event, context):
         if self.handler is None:
             raise ValueError("Cannot execute LambdaSnsEvent context without first configuring it")
 
         try:
             self.handler(LambdaSnsInputOutput(event['Records'][0]['Sns']['Message'], context))
         except Exception as e:
-            print('Failed message ' + record['MessageId'] + '. Error error: ' + str(e))
+            print('Failed message ' + event['Records'][0]['Sns']['MessageId'] + '. Error error: ' + str(e))
             raise e
 
-def lambda_sns_event(
+def lambda_sns(
     application,
     di_class=StandardDependencies,
     bindings=None,
     binding_classes=None,
     binding_modules=None,
     additional_configs=None,
 ):
     return build_context(
-        LambdaSnsEvent,
+        LambdaSns,
         application,
         di_class=di_class,
         bindings=bindings,
         binding_classes=binding_classes,
         binding_modules=binding_modules,
         additional_configs=additional_configs,
     )
```

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/di/standard_dependencies.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/di/standard_dependencies.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_api_gateway.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_elb.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_http_gateway.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_invocation.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_sns.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_sns.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 
     def json_body(self, required=True):
         if not self._record:
             if required:
                 raise ClientError("No SNS message found")
             return {}
 
-        try:
-            return json.loads(self._record)
-        except json.JSONDecodeError:
-            raise ClientError("SNS message was not valid JSON")
+        return self._record
 
     def get_request_method(self):
         raise NotImplementedError("Request methods don't exist in an SNS context")
 
     def get_script_name(self):
         raise NotImplementedError("Script names doesn't exist in an SNS context")
```

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/input_outputs/lambda_sqs_standard.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/input_outputs/lambda_sqs_standard.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/mocks/actions/ses.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/mocks/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/__init__.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/secrets/parameter_store.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/secrets/parameter_store.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/secrets/parameter_store_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/secrets/parameter_store_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/secrets/secrets_manager.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/src/clearskies_aws/secrets/secrets_manager_test.py` & `clear_skies_aws-1.5.6/src/clearskies_aws/secrets/secrets_manager_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.5/PKG-INFO` & `clear_skies_aws-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-aws
-Version: 1.5.5
+Version: 1.5.6
 Summary: clearskies bindings for working in AWS
 Home-page: https://github.com/cmancone/clearskies-aws
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

